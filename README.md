Odyssey question number 1343

# Introduction Challenge

###### ⚠️ Before starting this exercise, you must have finished some of the JavaScript quests

```quests
1262,1267,1268,1269, 1270, 1278, 1281, 1283, 1282, 1259
```

# 💪 Challenge

We are going to create a small website for cat adoption.

With dom manipulation, we can create easily some HTML elements without having to recreate them over and over.

In this exercise, you will see how we can generate cards from an array of objects easily.

In the following codesandbox, you will find a JavaScript file called `index.js` in this JavaScript file, you will find an array with a list of cats to adopt:

```javascript
const animalsToAdopt = [
  {
    name: "Lucky",
    picture: "https://placekitten.com/200/287"
  },
  {
    name: "Symba",
    picture: "https://placekitten.com/200/139"
  },
  {
    name: "Léo",
    picture: "https://placekitten.com/200/90"
  },
  {
    name: "Milo",
    picture: "https://placekitten.com/200/194"
  },
  {
    name: "Charly",
    picture: "https://placekitten.com/200/179"
  }
];
```

Our goal here is to create one card for each animal. 
That way, if we want to add a new animal to the list, we will simply have to add a new object in the array. 
 
For that, we need a function, because we don't want to run the same code over and over. To make this exercise more simple, we already created the function for you.

```javascript
function createCard(title, imageUrl) {
}
```

Each card will have a different `title` and a different `imageUrl`. 

To create new DOM elements, we have to use `document.createElement()`. We add a couple of example on how to proceed.

```javascript
const card = document.createElement("div");
card.classList.add("card");
cards.appendChild(card);
```


You have to create the element, then add the right class, and finally, add the element to its parent. 

Look at the example, and create the missing elements:

- cardBody: a div with the class `card-body` added to `card`
- cardTitle: a h2 with the class `card-title`, change the innerHTML with the `title` argument and add it to the `cardBody`
- cardButton: a button with the class `card-button`, the InnerHTML "Adopt Now" and add it to the `cardBody`

Once you've finished, now, create a for loop, that goes through the `animalsToAdopt` array and create one card for every element of the array.

```codesandbox
https://codesandbox.io/s/exercise-dom-forked-0vebn
```

# 🧐 Acceptance criteria

* [ ] The card contains all elements
* [ ] There is one card for each array element
