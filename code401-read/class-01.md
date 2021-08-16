# Map, Reduce, superagent, .Then, Async/Await


## Array.map
> Loops through an array and performs a given function on each element/index of the array. The result of a .map is a *new* array. It does not alter the original array.


## Array.reduce
> Utilizes a callback function to result in a single value. Reduce takes the arguments (accumulator, currentValue) and can take a second argument to set the initial value.

## superagent() **

> Code example with normal Promise .then() syntax:

```
request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });
   ```

> Code example with with async / await syntax:

```
const req = request
  .get('http://local')
  .auth('tobi', 'learnboost');
const res = yield req;
```

## JavaScript Promises

> JavaScript promises allow us to have a proxy for an object that has yet to be supplied. This is especially important for REST actions. The resulting value of a promise is tied to its success or failure.


## Are callback functions Asynchronous?

> Not by default. Callback functions can readily execute without waiting for a success/failure promise response.


** Code examples attributed to https://visionmedia.github.io/superagent/.