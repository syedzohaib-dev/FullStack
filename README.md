
# Emart

## Demo
https://tame-pink-indri-veil.cyclic.cloud/

This repository contains the code and resources for a full stack website developed by  Syed Zohaib Akhter  under the guidance of instructor Sir  Usama Usman.  The website is built using a combination of modern technologies, including React.js for the frontend, Express and Node.js for the backend, and MongoDB and Firebase for data storage and authentication.

## Features

- User registration and authentication system.
- Browse product by category, maal, or title.
- Search for product using hands.
- Add product to the shopping cart and proceed to checkout.
- Track order status and delivery information.
- Leave reviews and ratings for books.
- Manage user profiles and track order history.
- Admin panel for managing products, users, and orders.
- Responsive and user-friendly UI.




# Authors

- [syedzohaib](https://www.github.com/syedzohaib-dev)


# API REFRENCE
## Brands

```http
``` /api/create-brand
``` /api/get-all-brand
``` /api/get-brand-by-id
``` /api/update-brand
``` /api/delete-brand

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |

| `BrandName` | `string` | **Required*true*.  |
| `BrandImage` | `string` | **Required*true*. |


```

## Category

```http
``` /api/get-all-categories
``` /api/get-category-by-id
``` /api/create-category
``` /api/update-category
``` /api/delete-category

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |

| `CategoryName` | `string` | **Required*true*.  | unique*true*|
| `CategoryImage` | `string` | **Required*true*. |


```

## Mailer

```http
``` /api/sendmail
``` /api/sendfancymail


| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |

| `CategoryName` | `string` | **Required*true*.  | unique*true*|
| `CategoryImage` | `string` | **Required*true*. |


```

## Order

```http
``` /api/place-order
``` /api/get-all-orders
``` /api//track-order/:_id


| Parameter         | Type     | Description                |
| :--------         | :------- | :------------------------- |

| `customerName`    | `string` | **Required*true*.  | unique*true*|
| `customerEmail`   | `string` | **Required*true*. |
| `customerId`      | `string` | **Required*true*. |
| `customerContact` | `string` | **Required*true*. |
| `customerAddress` | `string` | **Required*true*. |
| `order`           | `array`  | **Required*true*. |
| `order_at`        | `default: Date.now` | **Required*true*. |

```

## Products

```http
``` /api/create-product
``` /api/get-all-products
``` /api/get-product-by-name
``` /api/get-product-by-id
``` /api/get-product-by-brand
``` /api/get-product-by-category
``` /api/update-product
``` /api/delete-product


| Parameter     | Type     | Description                |
| :--------     | :------- | :------------------------- |

| `ProductName` | `string` | **Required*true*.  |
| `description` | `string` | **Required*true*. |
| `price`       | `Number` | **Required*true*. |
| `category`    | `string` | **Required*true*. |
| `brand`       | `string` | **Required*true*. |
| `thumbnail`   | `string` | **Required*true*. |
| `imageArray`  | `[string]` | **Required*true*. |


```

## User

```http
``` /api/signup
``` /api/login
``` /api/getallusers
``` /api/getuserbyemail
``` /api/getuserbyid
``` /api/deleteuser
``` /api/updateuser


| Parameter     | Type     | Description                |
| :--------     | :------- | :------------------------- |

| `username`    | `string` | **Required*true*.  |
| `password`    | `string` | **Required*true*. |
| `email`       | `Number` | **Required*true*. |
| `role`        | `string` | **Required*true*. |
| `profile`     | `string` | **Required*true*. |
| `joining`     | `Date`   | **default : Date.now. |


```





# Role

### Admin

username :: Syed Zohaib ||
gmail :: zohaib@gmail.com ||
password  :: zohaib123

### User

username  :: asmat bhai ||
gmail  :: asmat@gmail.com ||
pass :: 12345678

username  :: ali bhai ||
gmail  :: ali@gmail.com ||
pass :: 12345678

### Guest

username  :: guest bhai ||
gmail  :: guest@gmail.com ||
pass :: 12345678
