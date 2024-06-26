
# Bread

A fullstack  social media web app with mern stack
## Tech Stack

**Client:** React , Redux , Chakra-ui  , React-Query , React-hook-form

**Server:** Node, Express , Mongodb , Joi (Data Validation) , JsonWebToken , Cloudinary , Bcryptjs


## API Reference

#### USERS API

```http
  GET /api/user/getuserdata/:username
  GET /api/user/profile/:query
  GET /api/user/recommended
  GET /api/user/feed
  POST /api/user/signup
  POST /api/user/login
  POST /api/user/logout
  POST /api/user/follow/:id
  PUT /api/user/update/:id
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `username` | `string` | **Required** name of user | 
| `query` | `string or mongodbId` | **Required** get user info  |
| `id` | `string` | **Required** userId for follow |
| `id` | `string` | **Required** userId for update profile |

#### POSTS API

```http
  GET /api/post/:username/post/:postId
  GET /api/post/:id
  GET /api/post/feed
  POST /api/post/create
  DELETE /api/post/:id
  PUT /api/post/like/:id
  PUT /api/post/reply/:id
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `username,postId`      | `string` | **Required**. Username and Post Id find all Post of |
| `id` | `string` | **Required** Post Id for find Post | 
| `id` | `string` | **Required** Post Id for Delete Post | 
| `id` | `string` | **Required** Post Id for like Post | 
| `id` | `string` | **Required** Post Id for Reply Post | 
