## Contact me
**Gilbert Joseph Smith III**

![@gjsmith3rd](https://avatars0.githubusercontent.com/gjsmith3rd?&s=128)

[Github](https://github.com/gjsmith3rd) | [FreeCodeCamp](http://www.freecodecamp.com/gjsmith3rd) |  [CodePen](http://codepen.io/gjsmith3rd/) | [LinkedIn](https://www.linkedin.com/in/gjsmith3rd) | [Blog/Site](https://gjsmith3rd.github.io/) | [E-Mail](mailto:contact@mobileCreature.com)

## Construct JavaScript Objects with Functions
Another way to create objects is with constructors. I particularly like them because them you can create more objects using them as a base.

```js
// Let's add the properties engines and seats to the car in the same way that the property wheels has been added below. They should both be numbers.
var Car = function() {
  this.wheels = 4;
  this.engines = 1;
  this.seats = 1;
};

var myCar = new Car();
```
