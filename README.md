```javascript
// OBJECT PROGRAMMING

avi = {
  walk: function() { console.log(this.name + ' is walking') },
  name: 'Avi'
}

avi.walk()
avi.lastName = 'Kaufman'

// PROTOTYPE PROGRAMMING

anotherAvi = {}
anotherAvi.__proto__ = avi
console.log(anotherAvi.name)

// CLASS BASED

function Person(name) {
  this.name = name
}

Person.prototype.walk = function() { console.log(this.name + ' is walking') }

console.log(new Person('bill'))

// confused? http://dmitry.baranovskiy.com/post/objects-in-javascript-part-ii
```
