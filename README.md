# T-Gadgetid restful api
This is my first restful api which I made using php native. The purpose of this api is make it easier for me to manage the content on the t-gadget.herokuapp.com.

## Tools & Stack
- [x] PHP Native (MVC)
- [x] remotemysql
- [x] firebase/php-jwt

## Endpoints
| about | url   | request method | auth | action |
| :--:  | :--:  |  :--:  |  :--:  |  :--:  |
| user activities | https://t-gadgetapi.herokuapp.com/user/:function_name  | `GET` `POST` `PUT` `DELETE` | api-key,token |<a href="/sub-readme/user-activities/README.md">detail</a>
| get data | https://t-gadgetapi.herokuapp.com/get/:function_name  | `GET` | api-key | <a href="/sub-readme/get-data/README.md">detail</a>
| add data | https://t-gadgetapi.herokuapp.com/add/:function_name  | `POST` | api-key,token | <a href="/sub-readme/add-data/README.md">detail</a>
| change data | https://t-gadgetapi.herokuapp.com/update/:function_name  | `PUT` | api-key,token | <a href="sub-readme/update-data/README.md">detail</a>
| delete data | https://t-gadgetapi.herokuapp.com/delete/:function_name  | `DELETE` | api-key,token | <a href="/sub-readme/delete-data/README.md">detail</a>