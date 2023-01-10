# Object and Symbol

-OBJECT

- Custom class

Declaration:

let person = {
firstName: 'John',
lastName: 'Adams',
age: 32,
partTime: false,
};

- Accessing the properties

  - dot syntax
    person.age = 33;
  - bracket syntax
    person['age'] = 33;

- SYMBOL

let mySymbol = Symbol()

-only objects that can access the [mySymbol] property are the ones who has access to the mySymbol variable.

let person = {
firstName: 'John',
lastName: 'Adams',
age: 32,
partTime: false,
[mySymbol]: 'secretInformation'
};

- METHODS - functions w/in the object

- this keyword = self

let person = {
firstName: 'John',
lastName: 'Adams',
age: 32,
partTime: false,
showInfo: function() {
showMessage(this.name)
}
};

- Passing Objects to functions

  - if you pass an object to a function. You can change its properties freely but if you pass a property (ie. string, integer, bool) to a function, you only change the parameter.

  let message = "hello";
  function changeMessage(message) {
  message = "hi"; // this changes the parameter not the outer variable
  }
  changeMessage(message);
  showMessage(message); // hello

---

function changeMessage(person) { //parameter is a pointer to the object and can access an external object
person.age++; // this changes the parameter not the outer variable
}
changeMessage(person);
showMessage(person.age);
