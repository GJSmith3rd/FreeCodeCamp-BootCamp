## Contact me
**Gilbert Joseph Smith III**

![@gjsmith3rd](https://avatars0.githubusercontent.com/gjsmith3rd?&s=128)

[Github](https://github.com/gjsmith3rd) | [FreeCodeCamp](http://www.freecodecamp.com/gjsmith3rd) |  [CodePen](http://codepen.io/gjsmith3rd/) | [LinkedIn](https://www.linkedin.com/in/gjsmith3rd) | [Blog/Site](https://gjsmith3rd.github.io/) | [E-Mail](mailto:contact@mobileCreature.com)

## Make Object Properties Private
Objects have their own attributes, called _properties_, and their own functions, called _methods_.

You can use the `this` keyword to reference _public properties and methods_ of the current objects. However, when You need to create private ones, so they are not accessible from the outside of the object.

For that, you just remove the keyword `this` from the object property or method declaration.

```js
var Bike = function() {
  speed = 100; // private
  function addUnit(value) { // private
    return value + "KM/H";
  }

  this.getSpeed = function () {  // public
    return addUnit(speed);
  };

};
```
