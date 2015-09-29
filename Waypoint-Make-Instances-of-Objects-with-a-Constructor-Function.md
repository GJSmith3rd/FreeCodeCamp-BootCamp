## Contact me
**Gilbert Joseph Smith III**

![@gjsmith3rd](https://avatars0.githubusercontent.com/gjsmith3rd?&s=128)

[Github](https://github.com/gjsmith3rd) | [FreeCodeCamp](http://www.freecodecamp.com/gjsmith3rd) |  [CodePen](http://codepen.io/gjsmith3rd/) | [LinkedIn](https://www.linkedin.com/in/gjsmith3rd) | [Blog/Site](https://gjsmith3rd.github.io/) | [E-Mail](mailto:contact@mobileCreature.com)

## Make Instances of Objects with a Constructor Function
A function that creates objects is called a _constructor_, my favorite way of creating objects when you have to create more than one of the same object. You can also edit the second object to add more properties if needed. This is called creating _instances_ of an object.

Each new instance of this object inherits all the properties and methods of your original object.

```js
var Car = function() {
   this.wheels = 4;
};

// New instance of Car object.
var myCar = new Car();

//Add the property "engines" to myCar, and make it a number.
myCar.engines = 1;
```
