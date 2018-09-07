# Verkefni 2
1. 
```javascript
let ingvar = {
	nafn: "Ingvar",
	heimasimi: 5431234,
	gsm: 8765434
};
console.log(ingvar.gsm);
```
2. console.log(family.parents.fathers[1]);
3.
```javascript
let breakfast = {
    name: "The Lumberjack",
    price: 9.95,
    ingredients: ["eggs", "sausage", "toast", "hashbrowns", "pancakes"]
};
```
4.
```javascipt
var savingsAccount = {
    balance: 1000,
    interestRatePercent: 1,
    deposit: function addMoney(amount) {
        if (amount > 0) {
            savingsAccount.balance += amount;
        }
    },
    withdraw: function removeMoney(amount) {
        var verifyBalance = savingsAccount.balance - amount;
        if (amount > 0 && verifyBalance >= 0) {
            savingsAccount.balance -= amount;
        }
    },
    // your code goes here
    printAccountSummary: function printSum() {
        return "Welcome! \nYour balance is currently $" + this.balance + " and your interest rate is " + this.interestRatePercent + "%.";
    }
};
console.log(savingsAccount.printAccountSummary());
```
5.
```javascript
let facebookProfile = {
    name: "Ingvar",
    friends: 123,
    messages: ["message1", "message2"],
    postMessage = function postMessage(message) {
        
    },
    deleteMessage = function deleteMessage(index) {
        
    },
    addFriend = function addFriend() {
        
    },
    removeFriend = function removeFriend() {
        
    }
};
```
6.
```javascript
function Pizza (staerd, alegg) {
  this.staerd = staerd;
  this.alegg = alegg;

  aleggsVerd = alegg.length * 495;
  lVerd = 1000;
  mVerd = 1500;
  sVerd = 2000;

  if (staerd === "Lítil") {
    return staerd + "(" + alegg + ") kr. " + (aleggsVerd+lVerd);
  } elif (staerd === "Miðstærð") {
    return staerd + "(" + alegg + ") kr. " + (aleggsVerd+mVerd);
  } else {
    return staerd + "(" + alegg + ") kr. " + (aleggsVerd+sVerd);
  }
}

let pizza1 = new Pizza("Lítil", ["ostur", "oregano"]);
let pizza2 = new Pizza("Miðstærð", ["ostur"]);
let pizza3 = new Pizza("Stór", ["pepperoni", "ostur", "oregano"]);
```
