# what-i-learned-week10

## CALLBACKS

asynchronous operations


#### readline.createInterface({ input: process.stdin, output: process.stdout })



fs.readline

### fs.writeFileSync()
#### Syntax:
```javascript
fs.writeFileSync( file, data, options )
```


corequire('readlline')
const interface - readlione.creatInterface({input: process.stdin,   
 output:provress/argv})
readlie reads the input rom the user.
method called create interface on it- coiler point code. retuns 
i want 

<hr>





# OBJECTS


keys and values  key value pairs.
syntax {} curly braces
- uses dot (.) notation.
- uses bracket [] notation  .
  bracket notation allows keys to be named with white spaces included.  
  dot notation doesn't.
  takes in a string, which is nice
  
- we can also change the values in our objects.
- objects are not ordered , numerically, alphabetically, etc.
- if we need an ordered list , use arrays.
- important to always have a trailing commma for easier modifications to objects.

- keys in objects can be deleted using javascirpt's 'delete'  
<hr>

## Create an OBJECT
**make an object**
```javascript
var myCar = {
    make: 'Ford',
    model: 'Mustang',
    year: 1969
};
```



We can immediately put some properties into {...} as “key: value” pairs: 

```javascript

let user = {     // an object
  name: "John",  // by key "name" store value "John"
  age: 30        // by key "age" store value 30
};
```
<hr>

## make a new property  
<hr>



## Accessing Object Properties
**You can access object properties in two ways:**

```javascript
objectName.propertyName      //dot notation  '.'
```

or

```javascript
objectName["propertyName"]    //bracket notation '[]'
```

**Example1**
```javascript
person.lastName;
```

Example2
```javascript
person["lastName"];
```





## Remove Property from an Object 
### delete operator
The **delete** operator **deletes** a property from an object:  
**delete** can **delete** a key from an object. thats all '**delete**' is for
#### Example
```javascript
var person = {
  firstName:"John",
  lastName:"Doe",
  age:50,
  eyeColor:"blue"
};

delete person.age;  // or delete person["age"];

// Before deletion: person.age = 50, after deletion, person.age = undefined
```
<hr>

## check whether a given key exists in an object
### You can do it by using the `in` operator

#### Example
```javascript
let learnLanguage = {
  javaScript: true,
  python: false,
  cSharp: true,
  java: true
};

let javaScriptExists = "javaScript" in learnLanguage;
console.log(javaScriptExists);
console.log("Learn Javascript? " + (learnLanguage["javascript"] ? "Yes" : "No"));
```
<hr>

### functions that take in Objects
#### Objects are mutable (mutation capability)

- we can change its properties
-  

<hr>

## JSON - What is JSON?
### **Javascript Object Notation**


like CSV, is a string, a bunch o f text that is readable by other people
starts with {} curly braces

- have data stored in a complex but portable way
- can handle : numbers, strings, booleans, objects, arrays, null
- cannot handle: undefined, methods, trailing commas, commented scripts
- portable means it can be read by other coding languages, even though it is made using javascript's syntax/format
- every JSON file is a valid Javascript Object.
- every Object is NOT valid JSON
- every string has to have "" quotes around it. NOTE double quotes has to be used NOT '' single quotes



<hr>

# New Methods Met in Week 10

### Object.keys()
### Object.values()

.reverse()
- mutates the original array from end to start
 
- typeof 
  The typeof operator returns a string indicating the type of the unevaluated operand.
  Syntax
The typeof operator is followed by its operand:
```javascript
typeof operand
typeof(operand)
```
**typeof EXAMPLE**
```javascript
console.log(typeof 42);
// expected output: "number"

console.log(typeof 'blubber');
// expected output: "string"

console.log(typeof true);
// expected output: "boolean"

console.log(typeof undeclaredVariable);
// expected output: "undefined"
```
<hr>
# Tips and Tricks

In terminal :
cd - - goes back one directiry(previous working environmnet.)
cat - show the contents of this file in terminal.

comment box extension in VS Code.
  Usage:  
-  highlight selected text
-  Shift + Cmd + p
-  transform to comment box

press `f12` while cursor is on the name of a function - vs code will take you directly to the function's declaration to help shed light on what the function contains.

- default a parameter when making a function 
```javascript
const makeDino = function (species, period, carnivore, extinct = false) {

}
```
<hr>

- **.endswith()**
- String.endsWith()  

  The endsWith() method determines whether a string ends with the characters of a specified string, returning true or false as appropriate.
**Syntax**
```javascript
str.endsWith(searchString[, length])
```
**EXAMPLE String.endsWith()**
```javascript
const str1 = 'Cats are the best!';

console.log(str1.endsWith('best', 17));
// expected output: true

const str2 = 'Is this a question';

console.log(str2.endsWith('?'));
// expected output: false
```
<hr>
- **JSON.parse()**
send that string into JSON.parse and recieve nad object as an putput.
  
- **JSON.stringify()**
   The JSON.stringify() method converts a JavaScript object or value to a JSON string,