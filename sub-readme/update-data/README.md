# UPDATE DATA ENDPOINT
<a href="../../README.md"><strong>« back to menu</strong></a>

<details open="open">
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="#11-update-socialmedia">update socialmedia</a></li>
    <li><a href="#12-update-countdown">update countdown</a></li>
    <li><a href="#13-update-product">update product</a></li>
    <li><a href="#14-update-statistic">update statistic</a></li>
  </ul>
</details>

## 1.1 update socialmedia
* **URL** <br>
https://t-gadgetapi.herokuapp.com/update/socialmedia
* **Request method** <br>
`PUT`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - link_tokopedia <br>
  - link_shopee    <br>
  - link_lazada    <br>
  - ourweb_link    <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "update socialmedia is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": {} }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.2 update countdown
* **URL** <br>
https://t-gadgetapi.herokuapp.com/update/countdown
* **Request method** <br>
`PUT`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - day    <br>
  - month  <br>
  - year   <br>
  - poster (file)(opsional)(max 1mb)<br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "update countdown is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": {} }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.3 update product
* **URL** <br>
https://t-gadgetapi.herokuapp.com/update/product
* **Request method** <br>
`PUT`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - product_id   <br>
  - product_name <br>
  - price        <br>
  - kategori     <br>
  - keyword      <br>
  - product_img (file)(opsional)(max 1 mb) <br>  
  - deskripsi    <br>
  - linktp       <br>
  - linksp       <br>
  - linklz       <br>
  - linkwa       <br>
  - stock        <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "update product with id .. is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.4 update statistic
* **URL** <br>
https://t-gadgetapi.herokuapp.com/update/statistic
* **Request method** <br>
`POST`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - for update value product viwers <br>
    * id 
  - for update value link visitor <br>
    * column (tokopedia/shopee/lazada/whatsapp/ourwebsite)
  - for update product link onclick <br>
    * id 
    * column (tokopedia/shopee/lazada/whatsapp)
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "data": {
          "table" : "",
          "column" : "",
          "current_value" : ""
        } 
      }
      ```
* **Error Response:**
    * **code :** 404 Not Found<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`
