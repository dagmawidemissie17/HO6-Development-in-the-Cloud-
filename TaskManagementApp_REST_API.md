# Task Management API: `api.tasks.testsite01.com`

 **Title** - REST API for a Task Management Application
- **Contact Email** - Dagmawi.Demissie@seattlecolleges.edu
- **Host** - api.tasks.testsite01.com
- **Schemes** - https


|Path |Create(POST)|Read(GET)|Update(PUT/PATCH)|DELETE(Delete)|
|:----|:----|:----|:----|:----|
|/users|Create User|List All Users|--|--|
| |Input: JSON|Input: --| | |
| |Output: UserID/User Object with the ID|Output: JSON Array| | |
| |HTTP Response Codes:|HTTP Response Codes:|HTTP Response Codes:|HTTP Response Codes:|
| |201: Post/Put Successful|200: OK|405: Method Not Allowed|405: Method Not Allowed|
| |400: Bad Request (Invalid Syntax)|401: Unknown and Unauthorized| | |
| |401: Unknown and Unauthorized|403: Known and Forbidden(Unauthorized)| | |
| |403: Known and Forbidden(Unauthorized)|500: Internal Server Error| | |
| |500: Internal Server Error|502: Bad Gateway| | |
| |502: Bad Gateway|503: Service Unavailable| | |
| |503: Service Unavailable| | | |
|/users/{user_id}|--|Show User|Change User|Remove User|
| | |Input: {user_id}|Input: {user_id} + User Object|Input: {user_id}|
| | |Output: User Object|Output: --|Output: --|
| |HTTP Response Codes:|HTTP Response Codes:|HTTP Response Codes:|HTTP Response Codes:|
| |405: Method Not Allowed|200: OK|201: Post/Put Successful|200: OK|
| | |401: Unknown and Unauthorized|401: Unknown and Unauthorized|401: Unknown and Unauthorized|
| | |403: Known and Forbidden(Unauthorized)|403: Known and Forbidden(Unauthorized)|403: Known and Forbidden(Unauthorized)|
| | |404: Not Found|404: Not Found|404: Not Found|
| | |500: Internal Server Error|500: Internal Server Error|500: Internal Server Error|
| | |502: Bad Gateway|502: Bad Gateway|502: Bad Gateway|
| | |503: Service Unavailable|503: Service Unavailable|503: Service Unavailable|
|/users/{user_id}/tasks|Create Task|Get all Tasks for User|--|--|
| |Input: {user_id} + JSON|Input: {user_id}| | |
| |Output: --|Output: JSON Array| | |
| |HTTP Response Codes:|HTTP Response Codes:|HTTP Response Codes:|HTTP Response Codes:|
| |201: Post/Put Successful|200: OK|405: Method Not Allowed|405: Method Not Allowed|
| |400: Bad Request (Invalid Syntax)|401: Unknown and Unauthorized| | |
| |401: Unknown and Unauthorized|403: Known and Forbidden(Unauthorized)| | |
| |403: Known and Forbidden(Unauthorized)|404: Not Found| | |
| |500: Internal Server Error|500: Internal Server Error| | |
| |502: Bad Gateway|502: Bad Gateway| | |
| |503: Service Unavailable|503: Service Unavailable| | |
|/users/{user_id}/tasks/{task_id}|--|Show Task for User|Change Task|Remove Task|
| | |Input: {user_id} + {task_id}|Input: {user_id} + {task_id} + JSON|Input: {user_id} + {task_id}|
| | |Output: Task Object|Output: --|Output: --|
| |HTTP Response Codes:|HTTP Response Codes:|HTTP Response Codes:|HTTP Response Codes:|
| |405: Method Not Allowed|200: OK|201: Post/Put Successful|200: OK|
| | |401: Unknown and Unauthorized|401: Unknown and Unauthorized|401: Unknown and Unauthorized|
| | |403: Known and Forbidden(Unauthorized)|403: Known and Forbidden(Unauthorized)|403: Known and Forbidden(Unauthorized)|
| | |404: Not Found|404: Not Found|404: Not Found|
| | |500: Internal Server Error|500: Internal Server Error|500: Internal Server Error|
| | |502: Bad Gateway|502: Bad Gateway|502: Bad Gateway|
| | |503: Service Unavailable|503: Service Unavailable|503: Service Unavailable|
