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

