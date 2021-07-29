# T-Gadgetid restful api
This is my first restful api which I made using php native. The purpose of this api is make it easier for me to manage the content on the t-gadget.herokuapp.com.

## Tools & Stack
- [x] PHP Native (MVC)
- [x] remotemysql
- [x] firebase/php-jwt

## Endpoints
| about | url   | request method | more info |
| :--:  | :--:  |  :--:  |  :--:  |
| user activities | https://t-gadgetapi.herokuapp.com/user/:function  | `GET` `POST` `PUT` `DELETE` | <a href="#user-activities">detail</a>
| get data | https://t-gadgetapi.herokuapp.com/get/:function  | `GET` | <a href="#get-data-endpoint">detail</a>
| add data | https://t-gadgetapi.herokuapp.com/add/:function  | `POST` | <a href="#add-data-endpoint">detail</a>
| change data | https://t-gadgetapi.herokuapp.com/update/:function  | `PUT` | <a href="#change-data-endpoint">detail</a>
| delete data | https://t-gadgetapi.herokuapp.com/delete/:function  | `DELETE` | <a href="#delete-data-endpoint">detail</a>

## Usage details

### 1. user activities endpoint

#### user register
* **URL** <br>
https://t-gadgetapi.herokuapp.com/user/register
* **Request method** <br>
`POST`
* **Params body** <br>
  [x] email    `text` <br> 
  [x] username `text` <br>
  [x] password `text` <br>
* **Success response**
    * **code :** 201 Created<br />
      **json :** `{ "success": true,"message": "User register is success!" }`
* **Error Response:**
    * **code :** 400 Bad Request<br />
      **json :** `{ "success": false,"message": {} }` <br/>
    OR<br/>
    * **code :** 500 Internal Server Error<br />
      **json :** `{ "success": false,"message": {} }`