# Back-End
## Schema

#### Users

| Field    | Type    | Notes                              |
| -------- | ------- | ---------------------------------- |
| id       | integer | _primary key_ and _autoincrements_ |
| email    | string  | _required_ and _unique_            |
| password | string  | _required_                         |
| username | string  | _required_                         |
| image_URL| string  |                                    |
| bio      | string  |                                    |

#### Stories

| Field     | Type    | Notes                                                                   |
| --------- | ------- | ----------------------------------------------------------------------- |
| id        | integer | _primary key_ and _autoincrements_                                      |
| name      | string  | _required_; name of the expat/story                                     |
| image_URL | string  | story image                                                             |
| location  | text    | _required_; story quote                                                 |
| content   | text    | _required_; story of the refugee                                        |
| author    | text    | author of the story                                                     |
| user_id   | integer | foreign key to link stories to user                                     |
