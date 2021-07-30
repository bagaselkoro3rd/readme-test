# T-Gadgetid restful api
This is my first restful api which I made using php native. The purpose of this api is make it easier for me to manage the content on the t-gadget.herokuapp.com.

## Tools & Stack
- [x] PHP Native (MVC)
- [x] remotemysql
- [x] firebase/php-jwt

## Endpoints
| about | url   | request method | more info |
| :--:  | :--:  |  :--:  |  :--:  |
| user activities | https://t-gadgetapi.herokuapp.com/user/:function  | `GET` `POST` `PUT` `DELETE` | <a href="#1-user-activities-endpoint">detail</a>
| get data | https://t-gadgetapi.herokuapp.com/get/:function  | `GET` | <a href="#get-data-endpoint">detail</a>
| add data | https://t-gadgetapi.herokuapp.com/add/:function  | `POST` | <a href="#add-data-endpoint">detail</a>
| change data | https://t-gadgetapi.herokuapp.com/update/:function  | `PUT` | <a href="#change-data-endpoint">detail</a>
| delete data | https://t-gadgetapi.herokuapp.com/delete/:function  | `DELETE` | <a href="#delete-data-endpoint">detail</a>

## Usage details

### 1. user activities endpoint
<details close="close">
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="#user-register">user register</a></li>
    <li><a href="#login">login</a></li>
    <li><a href="#user-session">user session</a></li>
    <li><a href="#user-update">user update</a></li>
    <li><a href="#logout">logout</a></li>
    <li><a href="#delete-account">delete account</a></li>
  </ul>
</details>

#### user register
* **URL** <br>
https://t-gadgetapi.herokuapp.com/user/register
* **Request method** <br>
`POST`
* **Params body** 
  - email     <br> 
  - username  <br>
  - password  <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "User register is success!" 
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": {} }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`
* **Notes:** <br>
*fetching, adding, updating and deleting data requires an api-key. so we have to register then login to get the api-key*

#### login
* **URL** <br>
https://t-gadgetapi.herokuapp.com/user/login
* **Request method** <br>
`POST`
* **Params body** 
  - username  <br>
  - password  <br>
* **Success response**
    * **code :** 200 Ok<br />
      **json  :** 
      ```
      { 
        "success": true,
        "data": {
            user_id:"",
            api_key:"",
            token:"",
            created_at:""
        } 
      }
      ```
* **Error Response:**
    * **code :** 401 Unauthorized<br />
      **json  :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json  :** `{ "success": false,"message": "" }`
* **Notes:** <br>
*token lifetime is 1 hour*