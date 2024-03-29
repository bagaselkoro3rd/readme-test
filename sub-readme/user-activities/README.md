# USER ACTIVITIES ENDPOINT
<a href="../../README.md"><strong>« back to menu</strong></a>

<details open="open">
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="#11-user-register">user register</a></li>
    <li><a href="#12-login">login</a></li>
    <li><a href="#13-user-session">user session</a></li>
    <li><a href="#14-user-update">user update</a></li>
    <li><a href="#15-logout">logout</a></li>
    <li><a href="#16-delete-account">delete account</a></li>
  </ul>
</details>

## 1.1 user register
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

## 1.2 login
* **URL** <br>
https://t-gadgetapi.herokuapp.com/user/login
* **Request method** <br>
`POST`
* **Params body** 
  - username  <br>
  - password  <br>
* **Success response**
    * **code :** 200 Ok<br />
      **json :** 
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
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`
* **Notes:** <br>
*token lifetime is 1 hour*

## 1.3 user session
* **URL** <br>
https://t-gadgetapi.herokuapp.com/user/session
* **Request method** <br>
`GET`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Success response**
    * **code :** 200 Ok<br />
      **json :** 
      ```
      { 
        "success": true,
        "data": {
            user_id:"",
            token_age:"",
        } 
      }
      ```
* **Error Response:**
    * **code :** 401 Unauthorized<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.4 user update
* **URL** <br>
https://t-gadgetapi.herokuapp.com/user/update
* **Request method** <br>
`PUT`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Params body** 
  - new_username  <br>
  - new_password  <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "update user is success!"
      }
      ```
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 401 Unauthorized<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.5 logout
* **URL** <br>
https://t-gadgetapi.herokuapp.com/user/logout
* **Request method** <br>
`DELETE`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Success response**
    * **code :** 202 Accepted<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "logout success"
      }
      ```
* **Error Response:**
    * **code :** 401 Unauthorized<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`

## 1.6 delete account
* **URL** <br>
https://t-gadgetapi.herokuapp.com/user/delete
* **Request method** <br>
`DELETE`
* **Request header** 
  - api-key  <br>
  - token  <br>
* **Success response**
    * **code :** 202 Accepted<br />
      **json :** 
      ```
      { 
        "success": true,
        "message": "delete account is success"
      }
      ```
* **Error Response:**
    * **code :** 401 Unauthorized<br />
      **json :** `{ "success": false,"message": "" }` <br/>

    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": "" }`