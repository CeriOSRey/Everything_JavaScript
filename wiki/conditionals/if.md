# if()

Declarations:
if (condition) {
do this
} else if (condition) {
do this
} else {
do this
}

Examples:

- always use 3 equal signs === (will also compare types) because == will convert the types so (1 == '1') is true
  if (5 === 5) {
  console.log('true');
  }

if ( 5>10) {
console.log('false');
}

if (5 >= 5) {
console.log('true');
}

---

let state = 'FL';
let taxPercent = 7;

if (state !== 'FL') {
taxPercent = 0;
}
