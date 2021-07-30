# DELETE DATA ENDPOINT
<a href="../../README.md"><strong>« back to menu</strong></a>

<details open="open">
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="#11-delete-product-category">delete product category</a></li>
    <li><a href="#12-delete-testimoni">delete testimoni</a></li>
    <li><a href="#13-delete-banner">delete banner</a></li>
    <li><a href="#14-delete-product">delete product</a></li>
  </ul>
</details>

## 1.1 delete product category
* **URL** <br>
https://t-gadgetapi.herokuapp.com/delete/category
* **Request method** <br>
`DELETE`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - category_id <br> 
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "delete category is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": {} }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.2 add testimoni
* **URL** <br>
https://t-gadgetapi.herokuapp.com/delete/testimoni
* **Request method** <br>
`DELETE`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - testi_id <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "delete testimoni is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": {} }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.3 add banner
* **URL** <br>
https://t-gadgetapi.herokuapp.com/delete/banner
* **Request method** <br>
`DELETE`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - banner_id <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "delete banner is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": {} }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.4 delete product
* **URL** <br>
https://t-gadgetapi.herokuapp.com/delete/product
* **Request method** <br>
`DELETE`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - product_id <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "delete product is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`