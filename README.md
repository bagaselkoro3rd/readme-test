# T-Gadgetid restful api
This is my first restful api which I made using php native. The purpose of this api is make it easier for me to manage the content on the t-gadget.herokuapp.com.

## 1. Tools & Stack
- [x] PHP Native (MVC)
- [x] remotemysql
- [x] firebase/php-jwt

## 2. Endpoints
| about | url   | method | more info |
| :--:  | :--:  |  :--:  |  :--:  |
| user activities | https://t-gadgetapi.herokuapp.com/user/:method  | `GET` `POST` `PUT` `DELETE` | <a href="#user-endpoint">detail</a>
| get specific data | https://t-gadgetapi.herokuapp.com/get/:method  | `GET` | <a href="#get-data-endpoint">detail</a>
| add some data | https://t-gadgetapi.herokuapp.com/add/:method  | `POST` | <a href="#add-data-endpoint">detail</a>
| change data info | https://t-gadgetapi.herokuapp.com/update/:method  | `PUT` | <a href="#change-data-endpoint">detail</a>
| delete data | https://t-gadgetapi.herokuapp.com/delete/:method  | `DELETE` | <a href="#delete-data-endpoint">detail</a>
