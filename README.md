# debounce-throttle-javascript

### Debouce
 Debounce execution of a function. Debouncing, unlike throttling,
 guarantees that a function is only executed a single time, either at the
 very beginning of a series of calls, or at the very end.
 
### Throttle
 Throttle execution of a function. Especially useful for rate limiting
 execution of handlers on events like resize and scroll.

## Install

```sh
npm install debounce-throttle-js
```

## Usage

### `debounce`

```js
const { debounce } = require("debounce-throttle-javascript");
/**
 * Using debounce() function
 * Param 1: Callback function to execute for debouncing behaviour eg. functionToExecute()
 * Parram 2: Time in milliseconds or debouncing interval eg. 500
 */
const debounceFunction = debounce(functionToExecute, 500);

```

### `throttle`

```js
const { throttle } = require("debounce-throttle-javascript");
/**
 * Using throttle() function
 * Param 1: Callback function to execute for throttling behaviour eg. functionToExecute()
 * Parram 2: Time in milliseconds or throttling interval eg. 300
 */
const throttleFunction = throttle(functionToExecute, 300);
```

## API

### throttle(callback, delay)

Returns: `Function`

Throttle execution of a function. Especially useful for rate limiting execution
of handlers on events like resize and scroll.

#### delay

Type: `Number`

A zero-or-greater delay in milliseconds. For event callbacks, values around 100
or 250 (or even higher) are most useful.

#### callback

Type: `Function`

A function to be executed after delay milliseconds. The `this` context and all
arguments are passed through, as-is, to `callback` when the throttled-function
is executed.

### debounce(callback, delay)

Returns: `Function`

Debounce execution of a function. Debouncing, unlike throttling, guarantees that
a function is only executed a single time, either at the very beginning of a
series of calls, or at the very end.

#### delay

Type: `Number`

A zero-or-greater delay in milliseconds. For event callbacks, values around 100
or 250 (or even higher) are most useful.

#### callback

Type: `Function`

A function to be executed after delay milliseconds. The `this` context and all
arguments are passed through, as-is, to `callback` when the debounced-function
is executed.
