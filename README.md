# JsHelpers

Just some JsHelpers I made for myself.

npm install jshelper

## Example

### ES6

```javascript
import JsHelper              = 'jshelper';
import Objects               = 'jshelper/Objects';
import { valueFromObject }   = 'jshelper/Objects';

var data = {
    person: {
        name: 'Ray Davis',
        age: 23,
    },
    job: 'idk',
};

const _jsHelper         = JsHelper.Objects.valueFromObject(data, 'person.name');
const _objects          = Objects.valueFromObject(data, 'person.name');
const _valueFromObject  = valueFromObject(data, 'person.name');

console.log(`JsHelper Output:           ${_jsHelper}`);
console.log(`Objects Output:            ${_objects}`);
console.log(`valueFromObject Output:    ${_valueFromObject}`);
```

### Non ES6

```javascript
const JsHelper              = require('jshelper').default;
```

## API

### JsHelper

JsHelper imports everything

### Objects

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### valueFromObject

This function search the item using a nexted string path

**Parameters**

-   `item` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** The object you want to search in
-   `propertyName` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** The path to the value seperated by dots (.). (optional, default `''`)

Returns **(any | [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** The found value or nothing

### Arrays

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### removeDupilcates

This function will remove all dupilcates from a array

**Parameters**

-   `array` **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)** The array to remove dupilcates from.

Returns **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)** The new array

### Dates

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### isValid

This function returns true if date is an instanceof Date

**Parameters**

-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date

Returns **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** if the date is an instanceof Date

#### daysInMonth

This function return the number of days in a month

**Parameters**

-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** The number of days in month or undefined if date is no valid
