# T-Gadgetid restful api
This is my first restful api which I made using php native. The purpose of this api is make it easier for me to manage the content on the t-gadget.herokuapp.com.

* 1. Tools & Stack
- [x] PHP Native (MVC)
- [x] remotemysql
- [x] firebase/php-jwt

* 2. Endpoints
| about | url   | request method | more info |
| :--:  | :--:  |  :--:  |  :--:  |
| user activities | https://t-gadgetapi.herokuapp.com/user/:function  | `GET` `POST` `PUT` `DELETE` | <a href="#user-endpoint">detail</a>
| get data | https://t-gadgetapi.herokuapp.com/get/:function  | `GET` | <a href="#get-data-endpoint">detail</a>
| add data | https://t-gadgetapi.herokuapp.com/add/:function  | `POST` | <a href="#add-data-endpoint">detail</a>
| change data | https://t-gadgetapi.herokuapp.com/update/:function  | `PUT` | <a href="#change-data-endpoint">detail</a>
| delete data | https://t-gadgetapi.herokuapp.com/delete/:function  | `DELETE` | <a href="#delete-data-endpoint">detail</a>

* 3. Usage details