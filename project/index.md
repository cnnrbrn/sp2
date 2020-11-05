# Semester Project 2

## Goal

To create an e-commerce website that has both customer-facing and admin sections. Both sections should be responsive and the website will be populated by a Strapi API supplied by Noroff.

## Brief

You are to build an e-commerce website. You can choose the theme of your website. It should follow the site architecture described below.

Design your website using your favourite tool. You will need to find a suitable logo. If you decide to create a logo yourself, do not spend too much time on it.

You must apply all that you have learned in your studies so far. The site must have a good user experience and UI design, following today's trends and design patterns.

Build a frontend with a home page, product list page and product detail page.

Build admin pages to create, update and delete products.

The website must be responsive on all devices.

Building a checkout and payment system is not a part of the project.

Level 1 is required.

Level 2 is optional.

## Strapi API

To start the API change directory to `api` install the npm dependecies and then run `npm run develop`

```bash
$ cd api
$ npm install
$ npm run develop
```

## User credentials

```bash
email: admin@admin.com
username: admin
password: Pass1234
```

## Level 1 (required)

### Customer-facing pages

#### Home page

The home page must include:

-   A hero banner with an image that is uploaded to Strapi.
-   A list of featured products. In Strapi each product has a featured flag that can be turned on or off. When the flag is on, the product should be displayed on the homepage.

#### Products page

The products page must include:

-   A list of all products added to Strapi. Each product must display its title, price and image. The product should link to its products detail page.
-   A search text box. When searching (filtering), only the products that include the searched text in their title or description should be listed.

#### Product details page

This page is reached by a user clicking on a product on the product list page. The product details page must include:

-   title
-   description
-   image
-   price
-   an add to cart button. This will toggle the product in and out of a cart array stored in local storage.

#### Cart/Basket page

The cart/basket page must display a list of all products added to the cart. Load the items that have been added to local storage and display them on the page. If the cart is empty display a message indicating this.

Each product in the cart must display:

-   title
-   price
-   a link to the product view page
-   image

After the list of products, display the total price of all the products in the cart.

Important: the cart page is not a checkout page. No payments or user details are required to be taken.

### Admin section

The admin section must include the following features.

#### Login/Logout

Create an admin login form that allows administrator users to login. Use local storage to keep the user logged in.

When logged in, display a logout button in the layout that logs the user out. Logging out should not clear the cart.

#### Add/edit products

Create form(s) that allow products to be added and edited. The form must allow the user to toggle whether a product is featured.

#### Product images

For adding/editing product images use either of these 2 methods:

1. Use a file upload field to upload images to Strapi, or
2. Use a text input that allows a URL to be entered. This allows an image from an external URL to be used as the product image.

#### Delete existing product

Allow products to be deleted. Before a product is deleted you must display a confirmation. The product should only be deleted if the user confirms. If the user cancels, the product must not be deleted.
