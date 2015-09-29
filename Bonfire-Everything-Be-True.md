## Contact me
**Gilbert Joseph Smith III**

![@gjsmith3rd](https://avatars0.githubusercontent.com/gjsmith3rd?&s=128)

[Github](https://github.com/gjsmith3rd) | [FreeCodeCamp](http://www.freecodecamp.com/gjsmith3rd) |  [CodePen](http://codepen.io/gjsmith3rd/) | [LinkedIn](https://www.linkedin.com/in/gjsmith3rd) | [Blog/Site](https://gjsmith3rd.github.io/) | [E-Mail](mailto:contact@mobileCreature.com)

# Details
- Difficulty: 2/5

Check if the predicate (second argument) returns truthy (defined) for all elements of a collection (first argument).

For this, check to see if the property defined in the second argument is present on every element of the collection.

Remember, you can access object properties through either dot notation or [] notation.

Remember to use [RSAP](http://www.freecodecamp.com/field-guide/how-do-i-get-help-when-I-get-stuck) if you get stuck. Try to pair program. Write your own code.

# Useful Links
- [Object.hasOwnProperty()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty)
- [Object.getOwnPropertyNames()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/getOwnPropertyNames)

# Problem Script:

```js
function every(collection, pre) {
  // Does everyone have one of these?
  return pre;
}

every([{'user': 'Tinky-Winky', 'sex': 'male'}, {'user': 'Dipsy', 'sex': 'male'}, {'user': 'Laa-Laa', 'sex': 'female'}, {'user': 'Po', 'sex': 'female'}], 'sex');
```

## Explanation:
The program needs to check if the second argument is a truthy element, and it must check this for each object in the first argument.

> In JavaScript, a truthy value is a value that translates to true when evaluated in a Boolean context. All values are truthy unless they are defined as falsy (i.e., except for false, 0, "", null, undefined, and NaN).

## Hint: 1
Remember to iterate through the first argument to check each object.

## Hint: 2
Only if all of them are truth will we return true, so make sure all of them check.

## Hint: 3
You could use loops or callbacks functions, there are multiple ways to solve this problem.

## My Code:

```js
function every(collection, pre) {
  // Create a counter to check how many are true.
  var counter = 0;

  // Check for each object
  for (var c in collection) {
    // If it has the same property or the same property value then add 1
    if (collection[c].hasOwnProperty(pre) || collection[c][pre] == pre) {
      counter++;
    }
  }

  // Outside the loop, check to see if we got true for all of them and return true or false
  if (counter == collection.length) {
    return true;
  } else
    return false;
}

every([{'user': 'Tinky-Winky', 'sex': 'male'}, {'user': 'Dipsy', 'sex': 'male'}, {'user': 'Laa-Laa',
'sex': 'female'}, {'user': 'Po', 'sex': 'female'}], 'sex');
```

## My Code Explanation:
- First I create a counter to check how many cases are actually true.
- Then check for each object if it it has the same property or the same property value. If true then add one to the counter.
- Outside the loop, I check to see if the counter variable has the same value as the length of **collection**, if true then return **true**, otherwise, return **false**

## [Go Home](https://github.com/Rafase282/My-FreeCodeCamp-Code/wiki)
