# Verkefni 3

1. Prototype-based programming is a style of object-oriented programming in which behaviour reuse (known as inheritance) is performed via a process of reusing existing objects via delegation that serve as prototypes
2. a. Þegar prototype er sleppt er function-ið sett beint í smiðinn. b. Book.prototype.getIsbn setur function-ið í object prototype-ið.
3. 
```javascript
function Geimflaugar(name, speed, life) {
  this.name = name;
  this.speed = speed;
  this.life = life;
}

let sseMajestic = new Geimflaugar ("SSE Majestic", 25, 10);
let templar = new Geimflaugar ("templar", 32, 10);
let zion = new Geimflaugar ("zion", 51, 10);

Geimflaugar.prototype.fly = function() {
  this.speed += 1
};

sseMajestic.fly();
templar.fly();
zion.fly();

let battlestar = {
  __proto__: sseMajestic,
  name: "battlestar",
  speed: 25,
  life: 15,
  setLife() {
      sseMajestic.life += 1;
    }
};

let babylon = {
  __proto__: sseMajestic,
  name: "babylon",
  speed: 25,
  life: 15,
  setLife() {
      sseMajestic.life += 1;
    }
};


battlestar.setLife();
babylon.setLife();
```
4. 
```javascript
class Geimflaugar {

  // Constructor
  constructor(name, speed, life) {
    this.name = name;
    this.speed = speed;
    this.life = life;
  }

  // Method
  fly() {
    this.speed += 1;
  }

}

class Undirflaugar extends Geimflaugar {
	setLife() {
		sseMajestic.life += 1;
	}
}

let sseMajestic = new Geimflaugar("SSE Majestic", 25, 10);
let templar = new Geimflaugar ("templar", 32, 10);
let zion = new Geimflaugar ("zion", 51, 10);

sseMajestic.fly();
templar.fly();
zion.fly();

let battlestar = new Undirflaugar("battlestar", 15, 15);
let babylon = new Undirflaugar("babylon", 15, 15);

battlestar.setLife();
babylon.setLife();

```
