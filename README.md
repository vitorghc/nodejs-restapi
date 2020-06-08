# nodejs-restapi
Example API rest using NodeJs



####  Dependencies:
* cors :  ^2.8.5
* express :  ^4.17.1
* mongoose :  ^5.9.17
* mongoose-paginate :  ^5.0.3
* require-dir:  ^1.2.0 

## Get Started

Clone project `https://github.com/vitorghcnodejs-restapi.git`.
 
##### How to use mongodb with docker:
docker mongodb pull
docker run --name mongodb -p 27017:27017 -d mongo

##### start application
npm run dev

##### how can i test API?

##### Create product:
POST localhost:3001/api/products
body: 
```
    {
        "title": "E-book Nodejs",
        "description": "Nodejs for dummies",
        "url": "http://www.node.org"
    }
```

##### Find products with paginated:
GET localhost:3001/api/products
GET localhost:3001/api/products?page=1

##### Find product by id:
GET localhost:3001/api/products/{id}

##### Update product:
PUT localhost:3001/api/products
body: 
```
    {
        "title": "E-book Nodejs"
    }
```
##### Delete product:
DELETE localhost:3001/api/products/{id}

