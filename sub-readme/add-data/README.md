# ADD DATA ENDPOINT
<a href="../../README.md"><strong>« back to menu</strong></a>

<details open="open">
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="#11-add-product-category">add product category</a></li>
    <li><a href="#12-add-testimoni">add testimoni</a></li>
    <li><a href="#13-add-banner">add banner</a></li>
    <li><a href="#14-add-product">add product</a></li>
  </ul>
</details>

## 1.1 add product category
* **URL** <br>
https://t-gadgetapi.herokuapp.com/add/category
* **Request method** <br>
`POST`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - category_name <br> 
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "add category is success!" 
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
https://t-gadgetapi.herokuapp.com/add/testimoni
* **Request method** <br>
`POST`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - img_testi (file)  <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "add testimoni is success!" 
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
https://t-gadgetapi.herokuapp.com/add/banner
* **Request method** <br>
`POST`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - banner_desktop (file)  <br>
  - banner_mobile  (file)  <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "add banner is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": {} }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.4 add product
* **URL** <br>
https://t-gadgetapi.herokuapp.com/add/product
* **Request method** <br>
`POST`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - product_name <br>
  - price        <br>
  - kategori     <br>
  - keyword      <br>
  - product_img (file) <br>  
  - deskripsi    <br>
  - linktp       <br>
  - linksp       <br>
  - linklz       <br>
  - linkwa       <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "add product is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`