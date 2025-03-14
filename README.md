# goit-js-hw-02

This repository contains JavaScript tasks for the GoIT homework assignment.

## Tasks

### Task 1: makeTransaction
This task involves creating a function `makeTransaction` that calculates the total amount for a transaction and checks if the customer has enough credits.

```js
function makeTransaction(quantity, pricePerDroid, customerCredits) {
    let totalAmount = quantity * pricePerDroid;

    return totalAmount <= customerCredits
      ? `You ordered ${quantity} droids worth ${totalAmount} credits!`
      : 'Insufficient funds!';
}
```


### Task 2: formatMessage
This task involves creating a function `formatMessage` that formats a message to a specified maximum length, adding an ellipsis if the message exceeds the length.

```js
function formatMessage(message, maxLength) {
    return message.length <= maxLength ? message : message.slice(0, maxLength) + "...";
}
```

### Task 3: checkForSpam
This task involves creating a function `checkForSpam` that checks if a message contains the words "spam" or "sale".

```js
function checkForSpam(message) {
    return message.toLowerCase().includes("spam") || message.toLowerCase().includes("sale");
}
```

### Task 4: getShippingCost
This task involves creating a function `getShippingCost` that returns the shipping cost for a given country.

```js
function getShippingCost(country) {
    switch (country) {
        case "China":
            return `Shipping to ${country} will cost ${100} credits`;
        case "Chile":
            return `Shipping to ${country} will cost ${250} credits`;
        case "Australia":
            return `Shipping to ${country} will cost ${170} credits`;
        case "Jamaica":
            return `Shipping to ${country} will cost ${120} credits`;
        default:
            return 'Sorry, there is no delivery to your country';
    }
}
```