# JsHelpers

Just some JsHelpers I made for myself.

npm install jshelper

## Example

### ES6

```javascript
import JsHelper              = 'jshelper';
import Objects               = 'jshelper/Objects';
import { find }   = 'jshelper/Objects';

var data = {
    person: {
        name: 'Ray Davis',
        age: 23,
    },
    job: 'idk',
};

const _jsHelper         = JsHelper.Objects.find(data, 'person.name');
const _objects          = Objects.find(data, 'person.name');
const _valueFromObject  = find(data, 'person.name');

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

#### find

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

This function returns the number of days in a month

**Parameters**

-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** The number of days in month or undefined if date is no valid

#### getMonthBounds

This function returns the start and end dates of the month

**Parameters**

-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A object containing the start and end dates or nothing

#### getWeekBounds

This function returns the start and end dates of the week

**Parameters**

-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A object containing the start and end dates or nothing

#### getWeekBoundsCentered

This function returns the start and end dates of the week centered around the date

**Parameters**

-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A object containing the start and end dates or nothing

#### getDayBounds

This function returns the start and end dates of the day

**Parameters**

-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A object containing the start and end dates or nothing

#### addToDate

This function returns a new date with the additions

**Parameters**

-   `$0` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)**
    -   `$0.years`   (optional, default `0`)
    -   `$0.months`   (optional, default `0`)
    -   `$0.days`   (optional, default `0`)
    -   `$0.hours`   (optional, default `0`)
    -   `$0.minutes`   (optional, default `0`)
    -   `$0.seconds`   (optional, default `0`)
    -   `$0.milliseconds`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A Date with the additions or nothing

#### addYears

This function returns a new Date with the added years

**Parameters**

-   `years`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A new Date with the addition or nothing

#### addMonths

This function returns a new Date with the added months

**Parameters**

-   `months`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A new Date with the addition or nothing

#### addWeeks

This function returns a new Date with the added weeks

**Parameters**

-   `weeks`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A new Date with the addition or nothing

#### addDays

This function returns a new Date with the added days

**Parameters**

-   `days`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A new Date with the addition or nothing

#### addHours

This function returns a new Date with the added hours

**Parameters**

-   `hours`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A new Date with the addition or nothing

#### addMinutes

This function returns a new Date with the added minutes

**Parameters**

-   `minutes`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A new Date with the addition or nothing

#### addSeconds

This function returns a new Date with the added seconds

**Parameters**

-   `seconds`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A new Date with the addition or nothing

#### addMilliseconds

This function returns a new Date with the added milliseconds

**Parameters**

-   `milliseconds`   (optional, default `0`)
-   `date` **[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)** any object that is an instanceof Date (optional, default `new Date()`)

Returns **([Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) \| [undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined))** A new Date with the addition or nothing
