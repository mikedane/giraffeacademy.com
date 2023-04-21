---
date: 2017-10-22T11:23:34-04:00
title: "AI Powered Shopping Cart"
seo_title: "AI Powered Shopping Cart | React | 🦒"
subheader:
     greeting: Javascript - Program the Web
     description: This course covers the basics of programming in Javascript & React. Work your way through the videos/articles and I'll teach you everything you need to know to make your website more responsive!
description: In this tutorial I'll show you how to build an AI powered shopping cart in React
author: 🦒
image: building-a-calculator.png
video: ShufCBZi_r8
url: /web-development/javascript/ai-shopping-cart/
weight: 30
---


<br />
Head over to https://alan.app/ Use promo code **MIKEDANE1000** to get 1000 free alan requests when you signup!


## Setting up the app

```bash
npx create-react-app menu-ai
cd menu-ai
```

## Building out a basic menu app

```jsx
const menuItems = [
   {name: "Angus Burger", price: 8.99, category: 'burger'},
   {name: "Tuna Steak Burger", price: 15.00, category: 'burger'},
   {name: "Bacon Burger", price: 11.50, category: 'burger'},
   {name: "Southwest Chicken Burger", price: 9.99, category: 'burger'},
   {name: "Mozzarella Burger", price: 12.50, category: 'burger'},
   {name: "Cesar Salad", price: 6.50, category: 'salad'},
   {name: "BBQ Chicken Salad", price: 13.99, category: 'salad'},
   {name: "Garden Salad", price: 9.99, category: 'salad'},
   {name: "Veggie Lasagna", price: 17.99, category: 'pasta'},
   {name: "Spaghetti & Meatballs", price: 17.99, category: 'pasta'},
   {name: "Fettuccine Alfredo", price: 17.99, category: 'pasta'},
];

const App = () => {
  const [products, setProducts] = useState([])
  const [cart, setCart] = useState([])
  
  return (
    <div className="App">
      {products.map((product) => (
        <div key={product.name}>
          {product.name} - {product.price} - {product.category}
        </div>
      ))}
      Cart:
      {cart.map((cartItem) => (
        <div key={cartItem.name}>
          {cartItem.name} - {cartItem.price} - {cartItem.category}
        </div>
      ))}
    </div>
  )
}
```

## Intents & Slots

```js
intent('(Hi|Hey|Yo) Alan, (my name is|you can call me) $(NAME)!', p => {
   p.play(`Hello ${p.NAME.value}!`); 
});
```

## Adding Alan to React

```bash
npm install @alan-ai/alan-sdk-web --save
```

```js
useEffect(() => {
    alanBtn({
      key:
        "e3a32cd64395a643bd3a03cee62943562e956eca572e1d8b807a3e2338fdd0dc/stage",
      onCommand: (commandData) => {
         console.log(commandData)
      },
    })
}, [])
```

## Getting Menu Items from Alan

Alan
```js
intent(
   '(show|open|what is on) (me|) (the|) menu',
   'what (do you have|can you offer|is available)',
   p => {
       p.play({command: 'getMenu', data: menuItems});
       p.play("Here are all the items we have");
   }
);
```

React
```js
if (commandData.command === "getMenu") {
 setProducts(commandData.data)
 console.log(commandData)
}
```

## Having Alan Order Menu Items

```js
intent(
   '(order|sort) by $(ORDER_BY name|price|category)',
   p => {
       const orderBy = p.ORDER_BY.value;
       let orderedMenuItems = menuItems;
       switch(orderBy){
           case 'name':
               orderedMenuItems = menuItems.sort((p1, p2) => p1.name.localeCompare(p2.name));
               break;
           case 'price':
               orderedMenuItems = menuItems.sort((p1, p2) => p1.price - p2.price);
               break;
           case 'category':
               orderedMenuItems = menuItems.sort((p1, p2) => p1.category.localeCompare(p2.category));
               break;
       }
       p.play({command: 'getMenu', data: orderedMenuItems});
       p.play(`Here are the items ordered by ${orderBy}`);
   }
);
```

## Asking for an item's price

```js
const itemsList = menuItems.map(m => m.name).join('|');

intent(`How much is (a|an) $(ITEM ${itemsList})`,
       `How much is (a|an) $(UNAVAILABLE_ITEM* .*)`, p => {
    if(p.UNAVAILABLE_ITEM){
        p.play("Sorry, that item is unavailable");
    } else {
        const itemName = p.ITEM.value;
        const item = menuItems.find(mi => mi.name.toLowerCase() === itemName.toLowerCase());
        p.play(`The ${item.name} is $${item.price}`);
    }
})
```

## Adding an item to the Cart

Alan
```js
intent(`Add $(ITEM ${itemsList}) to the cart`,
       `Add $(UNAVAILABLE_ITEM* .*) to the cart`, p => {
    if(p.UNAVAILABLE_ITEM){
        p.play("Sorry, that item is unavailable");
    } else {
        const itemName = p.ITEM.value;
        const item = menuItems.find(mi => mi.name.toLowerCase() === itemName.toLowerCase());
        p.play({command: 'addToCart', data: item});
        p.play(`Adding ${item.name} to the cart`);

    }
})
```

React
```js
else if (commandData.command === "addToCart") {
 setCart((currentCart) => [...currentCart, commandData.data])
}
```