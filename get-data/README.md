
# GET DATA ENDPOINT
* **URLs** <br>
    - socialmedia link <br/>
    https://t-gadgetapi.herokuapp.com/get/socialmedia <br/>
    - upcoming event <br/>
    https://t-gadgetapi.herokuapp.com/get/countdown <br/>
    - image banners <br/>
    https://t-gadgetapi.herokuapp.com/get/banners <br/>
    - image testimonies <br/>
    https://t-gadgetapi.herokuapp.com/get/testimonies <br/>
    - statstics <br/>
    https://t-gadgetapi.herokuapp.com/get/statistcs <br/>
    - product categories <br/>
    https://t-gadgetapi.herokuapp.com/get/categories <br/>
    - product keywords <br/>
    https://t-gadgetapi.herokuapp.com/get/keywords <br/>
    - all product <br/>
    https://t-gadgetapi.herokuapp.com/get/products <br/>
    - product by id <br/>
    https://t-gadgetapi.herokuapp.com/get/products?id=25 <br/>
    - product by category <br/>
    https://t-gadgetapi.herokuapp.com/get/products?category=category%20name <br/>
    - product by keyword <br/>
    https://t-gadgetapi.herokuapp.com/get/products?keyword=your%20word%20here <br/>
    - product using offset & limit <br/>
    https://t-gadgetapi.herokuapp.com/get/products/offset/limit <br/>
    NOTE: *offset and limit must integer*
    - product using offset, limit and filter <br/>
    https://t-gadgetapi.herokuapp.com/get/products/offset/limit/filterBy/filterVal <br/>
    NOTE: *filterBy is category and keyword*
* **Request method** <br>
`GET`
* **Request header** <br>
    - api-key  <br>
* **Success response**
    * **code :** 200 Ok<br />
      **json :** 
      ```
      { 
        "success": true,
        "data": "{ . . .}" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 401 Unauthorized<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 404 Not Found<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`