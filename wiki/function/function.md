# Functions

function name(parameter1,parameter2) {body};
name(parameter1, parameter2) // calling a function

Function Declaration:
function name() {...}

Example:

function showMessage() {
console.log('in a function');
}

---

- Function expression:

let fn = function optionalNameHere () {...}

---

- Passing a function as a parameter
  function getSecretCode(value) {
  let code = value \* 42
  return code;
  }
  console.log(getSecretCode(2)); // 84
