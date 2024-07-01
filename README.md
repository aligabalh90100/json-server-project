# JSON Server Project

Welcome to the JSON Server Project! This project simulates a RESTful API for an e-commerce application using JSON Server. It's ideal for development and testing without needing a full backend implementation.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Demo](#demo)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Server](#running-the-server)
- [API Endpoints](#api-endpoints)
- [Example Requests](#example-requests)
- [Sample Data](#sample-data)
-

## Introduction

This project provides a mock API with various endpoints for managing categories, products, wishlists, users, and orders. It's built with JSON Server to offer a lightweight solution for front-end development and testing.

## Features

- Simulates a RESTful API
- Comes with pre-populated sample data
- Quick setup and easy customization

## Demo

Access the demo [here](https://aligabalh90100.github.io/json-server-project/).

## Prerequisites

Before you begin, ensure you have Node.js installed. You can download it from [nodejs.org](https://nodejs.org/).

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/aligabalh90100/json-server-project.git
    cd json-server-project
    ```

2. **Install Dependencies**:
    ```bash
    npm install
    ```

## Running the Server

1. **Start JSON Server**:
    ```bash
    npm start
    ```

    The server will be available at `http://localhost:3000`.

2. **Access the API**:
    Open your browser and navigate to endpoints like `http://localhost:3000/categories` to see the data.

## API Endpoints

Here are the endpoints you can interact with:

- **Categories**
  - `GET /categories`: Retrieve all categories.
  - `GET /categories/:id`: Retrieve a specific category.

- **Products**
  - `GET /products`: Retrieve all products.
  - `GET /products/:id`: Retrieve a specific product.
  - `POST /products`: Add a new product.
  - `PUT /products/:id`: Update a specific product.
  - `DELETE /products/:id`: Delete a specific product.

- **Wishlist**
  - `GET /wishlist`: Retrieve all wishlist items.
  - `GET /wishlist/:id`: Retrieve a specific wishlist item.
  - `POST /wishlist`: Add a new wishlist item.
  - `PUT /wishlist/:id`: Update a specific wishlist item.
  - `DELETE /wishlist/:id`: Delete a specific wishlist item.

- **Users**
  - `GET /users`: Retrieve all users.
  - `GET /users/:id`: Retrieve a specific user.
  - `POST /users`: Add a new user.
  - `PUT /users/:id`: Update a specific user.
  - `DELETE /users/:id`: Delete a specific user.

- **Orders**
  - `GET /orders`: Retrieve all orders.
  - `GET /orders/:id`: Retrieve a specific order.
  - `POST /orders`: Add a new order.
  - `PUT /orders/:id`: Update a specific order.
  - `DELETE /orders/:id`: Delete a specific order.

## Example Requests

Here are some example requests you can try using `curl`:

### Fetch All Categories
```bash
curl http://localhost:3000/categories
curl http://localhost:3000/products/1
curl -X PUT -H "Content-Type: application/json" -d '{"title": "Updated Product", "price": 150}' http://localhost:3000/products/1
```

## Sample Data

The `db.json` file in this project contains sample data that simulates the structure of a typical e-commerce database. Below are some snippets from this file, showcasing categories, products, and users.

### Categories

This section lists different categories available in the store. Each category includes an ID, title, prefix, and image URL.

```json
[
  {
    "id": 1,
    "title": "men",
    "prefix": "men",
    "img": "https://cdn-eu.dynamicyield.com/api/9876644/images/cfb357649428__hp-w12-22032022-h_m-men.jpg"
  },
  {
    "id": 2,
    "title": "women",
    "prefix": "women",
    "img": "https://cdn-eu.dynamicyield.com/api/9876644/images/30d354267a09b__hp-w12-22032022-h_m-women_dresses.jpg"
  },
  {
    "id": 3,
    "title": "kids",
    "prefix": "kids",
    "img": "https://cdn-eu.dynamicyield.com/api/9876644/images/37d243d334c63__hp-w12-22032022-h_m-kids1.jpg"
  },
  {
    "id": 4,
    "title": "baby",
    "prefix": "baby",
    "img": "https://cdn-eu.dynamicyield.com/api/9876644/images/28948d47ae6e8__h_m-w39-28092022-4066c-1x1.jpg"
  },
  {
    "id": 5,
    "title": "sport",
    "prefix": "sport",
    "img": "https://cdn-eu.dynamicyield.com/api/9876644/images/1dda9ae79a671__h_m-w40-06102022-7416b-1x1.jpg"
  }
]
```
### Products

This section details various products available in the store. Each product includes an ID, title, price, category prefix, image URL, and maximum quantity.


```json
[
  {
    "id": 1,
    "title": "Jersey top",
    "price": 249,
    "cat_prefix": "men",
    "img": "https://eg.hm.com/assets/styles/HNM/14482498/6103a8463876770c30cdba3535b7be1f333315fe/2/image-thumb__3464789__product_listing/cb91f8f128ac2125e0ec3a008a2e8d2497d15434.jpg",
    "max": 4
  },
  {
    "id": 2,
    "title": "Regular Fit Jersey top",
    "price": 229,
    "cat_prefix": "men",
    "img": "https://eg.hm.com/assets/styles/HNM/14482498/6103a8463876770c30cdba3535b7be1f333315fe/2/image-thumb__3464789__product_listing/cb91f8f128ac2125e0ec3a008a2e8d2497d15434.jpg",
    "max": 4
  },
  {
    "id": 3,
    "title": "Cotton polo shirt",
    "price": 200,
    "cat_prefix": "men",
    "img": "https://eg.hm.com/assets/styles/HNM/13994073/eeb1d90c4764366000eb8b8571396e81f0de5c44/2/image-thumb__3142108__product_listing/4d6db9e8f936d3d82b13bc5861b0310fa214c74d.jpg",
    "max": 3
  },
  {
    "id": 4,
    "title": "Cotton t-shirt",
    "price": 100,
    "cat_prefix": "women",
    "img": "https://eg.hm.com/assets/styles/HNM/13650519/6cc34f51caee1d6cfe776b933d667075fa30d90d/2/image-thumb__2888777__product_listing/16c27492b022ac2eef03853f85d5b279a29ebeed.jpg",
    "max": 2
  },
  {
    "id": 5,
    "title": "Sweatshirt shorts",
    "price": 300,
    "cat_prefix": "women",
    "img": "https://eg.hm.com/assets/styles/HNM/12652575/3e316aab8ce1b596545d144d0efd362975b3856f/2/image-thumb__1998684__product_listing/48756e509aa05341e4a618ba4c1b0a5ce24ebcae.jpg",
    "max": 3
  },
  {
    "id": 6,
    "title": "Velour top",
    "price": 300,
    "cat_prefix": "kids",
    "img": "https://eg.hm.com/assets/styles/HNM/14478215/543d925539f4a3b92a79df2dfe46d5d481e1c7ae/2/image-thumb__3463278__product_listing/c1417d02c7a93e6d2aca7965003b4f7d490f0ae8.jpg",
    "max": 2
  },
  {
    "id": 9,
    "title": "Pile all-in-one suit with ears",
    "price": 500,
    "cat_prefix": "baby",
    "img": "https://eg.hm.com/assets/styles/HNM/10803913/c334b471ad8f564ed1b5dd410c95d94544ee0904/2/image-thumb__1594613__product_listing/5941e37dccc9b0172ac2ab7c266c1cd794cb547f.jpg",
    "max": 2
  },
  {
    "id": 17,
    "title": "Regular Fit football shirt",
    "price": 449,
    "cat_prefix": "sport",
    "img": "https://eg.hm.com/assets/styles/HNM/14472541/cb9d35f1480ce5c8b0be39ad7fd35ab9f8004ce0/2/image-thumb__3453052__product_listing/70408034bd9792a93abbc8ad322565337f535e24.jpg",
    "max": 2
  }
]
```

### Users

This section lists users in the system, including their email, password (hashed for security), first name, last name, and ID.

```json
[
 {
    "email": "aligabalh90100@gmail.com",
    "password": "$2a$10$PRMaXT8MxsL1R5TAOTEuG.wkphTSABptrrGwb6xCqy/eRg9XsyW9C",
    "firstName": "ali",
    "lastName": "mohamed",
    "id": 1
  },
  {
    "email": "mateja.bezamovski@gmail.com",
    "password": "$2a$10$iAcaudgK9/Ibtd3TPNcQ2eZ.lyWcgP71ujsyNmFKZoyVN0o.fZ7ju",
    "firstName": "ali",
    "lastName": "mohamed",
    "id": 2
  }
]
```

### Wishlists

This section details user wishlists, linking users to the products they have added to their wishlists.

```json
[
 {
    "userId": 2,
    "productId": 5,
    "id": 1
  },
  {
    "userId": 2,
    "productId": 4,
    "id": 2
  },
  {
    "userId": 1,
    "productId": 6,
    "id": 3
  },
  {
    "userId": 1,
    "productId": 3,
    "id": 4
  },
  {
    "userId": 1,
    "productId": 2,
    "id": 5
  },
  {
    "userId": 1,
    "productId": 1,
    "id": 6
  }
]
```

### Orders

This section lists orders placed by users, including the user ID, items ordered, subtotal, and order ID.

```json
[
 {
    "userId": 1,
    "items": [
      {
        "title": "Jersey top",
        "id": 1,
        "img": "https://eg.hm.com/assets/styles/HNM/14482498/6103a8463876770c30cdba3535b7be1f333315fe/2/image-thumb__3464789__product_listing/cb91f8f128ac2125e0ec3a008a2e8d2497d15434.jpg",
        "price": 249,
        "quantity": 2
      },
      {
        "title": "Regular Fit Jersey top",
        "id": 2,
        "img": "https://eg.hm.com/assets/styles/HNM/14482498/6103a8463876770c30cdba3535b7be1f333315fe/2/image-thumb__3464789__product_listing/cb91f8f128ac2125e0ec3a008a2e8d2497d15434.jpg",
        "price": 229,
        "quantity": 1
      }
    ],
    "subtotal": 727,
    "id": 1
  },
  {
    "userId": 2,
    "items": [
      {
        "title": "Sweatshirt shorts",
        "id": 5,
        "img": "https://eg.hm.com/assets/styles/HNM/12652575/3e316aab8ce1b596545d144d0efd362975b3856f/2/image-thumb__1998684__product_listing/48756e509aa05341e4a618ba4c1b0a5ce24ebcae.jpg",
        "price": 300,
        "quantity": 1
      },
      {
        "title": "Cotton polo shirt",
        "id": 3,
        "img": "https://eg.hm.com/assets/styles/HNM/13994073/eeb1d90c4764366000eb8b8571396e81f0de5c44/2/image-thumb__3142108__product_listing/4d6db9e8f936d3d82b13bc5861b0310fa214c74d.jpg",
        "price": 200,
        "quantity": 2
      }
    ],
    "subtotal": 700,
    "id": 2
  }
]
```
