# TOPICK

**โดย** 
1. นางสาวกานต์รวี วารินทร์ศิริกุล 6210402348
2. นายณรงค์ฤทธ์ ธรรมปาโล 6210402402
3. นายนิรัตศัย หารี 6210407455

## Project setup
```
npm install
```

## Frontend
https://github.com/Ford-Narongrit/midterm-webtech-frontend/

## Develop
```
npm run develop
```

## .tmp
เพิ่มไฟล์ **.tmp** 

## API Routes

* Create account : `POST /api/users`\
`body = { Text:username, Email:email, Password:password, Text:name }`\
`headers = { Authorization: 'Bearer <jwt>', content-type : application/json}`

**chatboard**

_1. post_
* Create post : `POST /api/posts`\
`body = { Text:text, Number:like, Text:title, User:id, Comment:[id] }`\
`headers = { Authorization: 'Bearer <jwt>', content-type : application/json}`

* Get by post id  : `GET /api/posts/:id`\
`Params =  id:id`

_2. comment_
* Create comment on post : `POST /api/comments`\
`body = { Text:text, Number:like, Posts:id, User:id }`\
`headers = { Authorization: 'Bearer <jwt>', content-type : application/json}`

* Get by comment id  : `GET /api/comments/:id`\
`Params: id:id`

**reward**
* Create reward : `POST /api/rewards` \
`body = { Text:name, Rich text:describtion, Number:remain, Number:point_used, Text: image_path, User:[id] }`\
`headers = { Authorization: 'Bearer <jwt>', content-type : application/json}`

* Get by reward id  : `GET /api/rewards/:id`\
`Params: id:id`

* Get all rewards and information : `GET /api/rewards`

* Update reward information : `PUT /api/rewards/:id`\
`body = { Text:name, Rich text:describtion, Number:remain, Number:point_used, Text: image_path }`\
`headers = { Authorization: 'Bearer <jwt>', content-type : application/json}`

* Delete reward : `DELETE /api/rewards/:id`
`Params: id:id`

**user-points**
* Get all user points information :  `GET /api/user-points`

**user-rewards**
* Get all user rewards information :  `GET /api/user-rewards`
