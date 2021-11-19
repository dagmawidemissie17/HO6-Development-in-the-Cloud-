# Task Management API: `api.tasks.testsite01.com`

 **Title** - REST API for a Task Management Application
- **Contact Email** - Dagmawi.Demissie@seattlecolleges.edu
- **Host** - api.tasks.testsite01.com
- **Schemes** - https

## Paths

| ****                                   | **POST**                                 | **GET**                                  | **PUT/PATCH**                               | **DELETE**                               |
|----------------------------------------|------------------------------------------|------------------------------------------|---------------------------------------------|------------------------------------------|
| /users                                 | Create User                              | List All Users                           | \-\-                                        | \-\-                                     |
|                                        | Input: JSON                              | Input: \-\-                              |                                             |                                          |
|                                        | Output: UserID/User Object with the ID   | Output: JSON Array                       |                                             |                                          |
|                                        | HTTP Response Codes:                     | HTTP Response Codes:                     | HTTP Response Codes:                        | HTTP Response Codes:                     |
|                                        | 201: Post/Put Successful                 | 200: OK                                  | 405: Method Not Allowed                     | 405: Method Not Allowed                  |
|                                        | 400: Bad Request \(Invalid Syntax\)      | 401: Unknown and Unauthorized            |                                             |                                          |
|                                        | 401: Unknown and Unauthorized            | 403: Known and Forbidden\(Unauthorized\) |                                             |                                          |
|                                        | 403: Known and Forbidden\(Unauthorized\) | 500: Internal Server Error               |                                             |                                          |
|                                        | 500: Internal Server Error               | 502: Bad Gateway                         |                                             |                                          |
|                                        | 502: Bad Gateway                         | 503: Service Unavailable                 |                                             |                                          |
|                                        | 503: Service Unavailable                 |   
|                                             |                                          |
| /users/\{user\_id\}                    | \-\-                                     | Show User                                | Change User                                 | Remove User                              |
|                                        |                                          | Input: \{user\_id\}                      | Input: \{user\_id\} \+ User Object          | Input: \{user\_id\}                      |
|                                        |                                          | Output: User Object                      | Output: \-\-                                | Output: \-\-                             |
|                                        | HTTP Response Codes:                     | HTTP Response Codes:                     | HTTP Response Codes:                        | HTTP Response Codes:                     |
|                                        | 405: Method Not Allowed                  | 200: OK                                  | 201: Post/Put Successful                    | 200: OK                                  |
|                                        |                                          | 401: Unknown and Unauthorized            | 401: Unknown and Unauthorized               | 401: Unknown and Unauthorized            |
|                                        |                                          | 403: Known and Forbidden\(Unauthorized\) | 403: Known and Forbidden\(Unauthorized\)    | 403: Known and Forbidden\(Unauthorized\) |
|                                        |                                          | 404: Not Found                           | 404: Not Found                              | 404: Not Found                           |
|                                        |                                          | 500: Internal Server Error               | 500: Internal Server Error                  | 500: Internal Server Error               |
|                                        |                                          | 502: Bad Gateway                         | 502: Bad Gateway                            | 502: Bad Gateway                         |
|                                        |                                          | 503: Service Unavailable                 | 503: Service Unavailable                    | 503: Service Unavailable   
|
| /users/\{user\_id\}/tasks              | Create Task                              | Get all Tasks for User                   | \-\-                                        | \-\-                                     |
|                                        | Input: \{user\_id\} \+ JSON              | Input: \{user\_id\}                      |                                             |                                          |
|                                        | Output: \-\-                             | Output: JSON Array                       |                                             |                                          |
|                                        | HTTP Response Codes:                     | HTTP Response Codes:                     | HTTP Response Codes:                        | HTTP Response Codes:                     |
|                                        | 201: Post/Put Successful                 | 200: OK                                  | 405: Method Not Allowed                     | 405: Method Not Allowed                  |
|                                        | 400: Bad Request \(Invalid Syntax\)      | 401: Unknown and Unauthorized            |                                             |                                          |
|                                        | 401: Unknown and Unauthorized            | 403: Known and Forbidden\(Unauthorized\) |                                             |                                          |
|                                        | 403: Known and Forbidden\(Unauthorized\) | 404: Not Found                           |                                             |                                          |
|                                        | 500: Internal Server Error               | 500: Internal Server Error               |                                             |                                          |
|                                        | 502: Bad Gateway                         | 502: Bad Gateway                         |                                             |                                          |
|                                        | 503: Service Unavailable                 | 503: Service Unavailable                 |                                             |  
|
| /users/\{user\_id\}/tasks/\{task\_id\} | \-\-                                     | Show Task for User                       | Change Task                                 | Remove Task                              |
|                                        |                                          | Input: \{user\_id\} \+ \{task\_id\}      | Input: \{user\_id\} \+ \{task\_id\} \+ JSON | Input: \{user\_id\} \+ \{task\_id\}      |
|                                        |                                          | Output: Task Object                      | Output: \-\-                                | Output: \-\-                             |
|                                        | HTTP Response Codes:                     | HTTP Response Codes:                     | HTTP Response Codes:                        | HTTP Response Codes:                     |
|                                        | 405: Method Not Allowed                  | 200: OK                                  | 201: Post/Put Successful                    | 200: OK                                  |
|                                        |                                          | 401: Unknown and Unauthorized            | 401: Unknown and Unauthorized               | 401: Unknown and Unauthorized            |
|                                        |                                          | 403: Known and Forbidden\(Unauthorized\) | 403: Known and Forbidden\(Unauthorized\)    | 403: Known and Forbidden\(Unauthorized\) |
|                                        |                                          | 404: Not Found                           | 404: Not Found                              | 404: Not Found                           |
|                                        |                                          | 500: Internal Server Error               | 500: Internal Server Error                  | 500: Internal Server Error               |
|                                        |                                          | 502: Bad Gateway                         | 502: Bad Gateway                            | 502: Bad Gateway                         |
|                                        |                                          | 503: Service Unavailable                 | 503: Service Unavailable                    | 503: Service Unavailable                 |


