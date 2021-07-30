# T-Gadgetid restful api
This is my first restful api which I made using php native. The purpose of this api is make it easier for me to manage the content on the t-gadget.herokuapp.com.

## Tools & Stack
- [x] PHP Native (MVC)
- [x] remotemysql
- [x] firebase/php-jwt

## Endpoints
| about | url   | request method | details |
| :--:  | :--:  |  :--:  |  :--:  |
| user activities | https://t-gadgetapi.herokuapp.com/user/:function  | `GET` `POST` `PUT` `DELETE` | <a href="/sub-readme/user-activities/README.md">detail</a>
| get data | https://t-gadgetapi.herokuapp.com/get/:function  | `GET` | <a href="/sub-readme/get-data/README.md">detail</a>
| add data | https://t-gadgetapi.herokuapp.com/add/:function  | `POST` | <a href="/sub-readme/add-data/README.md">detail</a>
| change data | https://t-gadgetapi.herokuapp.com/update/:function  | `PUT` | <a href="#change-data-endpoint">detail</a>
| delete data | https://t-gadgetapi.herokuapp.com/delete/:function  | `DELETE` | <a href="/sub-readme/delete-data/README.md">detail</a>