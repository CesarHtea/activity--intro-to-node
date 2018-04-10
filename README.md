# Intro to Node.JS

## Create a server using `http` Node module

### Setup Instructions

In Terminal:

```sh
# (1) navigate to your activities directory
$ cd ~/Documents/muktek/activities

# (2) Create a activity--intro-to-nodejs project
$ mkdir activity--intro-to-nodejs

$ cd activity--intro-to-nodejs

# (3) Create the main file (`server.js`)
$ touch server.js
```

In File:

#### 1. Import `http` Node module

#### 2. Use `createServer` function to create a web server

#### 3. Configure and use the PORT 3000 to run our application

#### 4. Configure the following routes:

```
/                  : 'Home page'
/about             : 'About page'
/api/products      : products (in JSON format)
/api/orders        : orders (in JSON format)
```

###### Products
```js
const products = {
  data: [{
    id: 1,
    name: 'Cookies',
    price: '12.39'
  }, {
    id: 2,
    name: 'Halls',
    price: '9.88'
  }, {
    id: 3,
    name: 'Orange Juice',
    price: '20.00'
  }]
};
```

###### Orders
```js
const orders = {
  data: [{
    id: 1,
    date:
    products: [{
      id: 2,
      name: 'Halls',
      quantity: 2
    }, {
      id: 1,
      name: 'Cookies',
      quantity: 1
    }],
    total: '25.00'
  }, {
    id: 2,
    date:
    products: [{
      id: 1,
      name: 'Cookies',
      quantity: 4
    }],
    total: '26.78'
  }]
};
```
