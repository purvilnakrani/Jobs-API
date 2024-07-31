# `JOBS API`  ( Backend )

#### Project Setup

## `Installation`

If you want to work on this project , clone this repo

```bash
git clone "https://github.com/purvilnakrani/Jobs-API.git"

```

Open this project on your local IDE and in the terminal do this commands one by one

 ```
 npm install
 npm run start
```

Before running code do not forget to change database connection url, To get that url go to mongodb atlas cluster -> connect -> driver
Ex:- `MONGODBURI: mongodb+srv://<user_name>:<password>@mongodb_connection_string/database_name`


## `API Reference`

Base URL
```https
localhost:3000/api/v1
```

- get list of all products from store
```http
  GET /products
```
- get list of static products from store
```http
  GET /products/static
```
- Url query searching
```http
  GET /products?name=bench&featured=true
```
- Url query searching (page)
```http
  GET /products?featured=false&page=2
```
- Url query searching (enum)
```http
  GET /products?featured=false&company=ikea
```
- Url query searching (Numeric filters)
 ```http
  GET /products?numericFilters=price<100,rating>=4
```

## `Tech Stack`

**Server:** Node, Express
**database:** MongoDB
