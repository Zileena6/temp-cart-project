## Figma URL

[Cart](https://www.figma.com/file/5AwKjnWuM6BhRYmxdQFpky/Cart?node-id=0%3A1&t=lfaO4zazTd7nqF1q-1)

#### Setup

```sh

npm install
```

```sh
npm run dev
```


#### Global Context and useReducer

Set up global context and immediately create a general setup for useReducer. Create two files, one for reducer and one for actions.

#### Functionalities

Implement these functionalities in the reducer and actions files, and make them available in the global context.

Clear Cart - an action that clears the entire cart.
Remove Item - an action that removes a specific item from the cart.
Increase Amount - an action that increases the quantity of a specific item in the cart.
Decrease Amount - an action that decreases the quantity of a specific item in the cart.

#### Calculate Totals

Calculate Totals - a function that calculates the total cost of items in the cart.

#### Data Structure Options

Using an array to store shopping cart data may not be the best option because it can be less efficient for lookups and updates, especially for larger datasets. Arrays are also less flexible than Maps when it comes to associating values with unique identifiers.


The downsides of using an object to store shopping cart data include the risk of unintended property overwriting or unexpected behavior when iterating over inherited properties. Additionally, objects can only use string keys, which can be limiting if you need to use non-string keys. Deleting properties from an object can also be tricky, especially when dealing with inherited properties.

- new Map()

For a shopping cart application, using a new Map() to store the cart data is beneficial because it allows for efficient lookups and updates based on unique product IDs. Using a Map can also ensure that each item in the cart has a unique identifier and can easily be updated or removed without affecting other items in the cart.

#### Map

A Map is a built-in data structure in JavaScript that allows you to store key-value pairs, where both the keys and values can be any data type. Here's a simple example:

#### JS Nuggets Video

[Array.from](https://www.youtube.com/watch?v=zg1Bv4xubwo&list=PLnHJACx3NwAfRUcuKaYhZ6T5NRIpzgNGJ&index=11)


