# [DalekJS](http://dalekjs.com/) Cheat Sheet v0.0.8

## Installation

1. Install node
1. Install globally "DalekJS Command Line Tools" `npm install dalek-cli -g`
1. Install locally "DalekJS" in your testing directory `npm install dalekjs --save-dev`

## Test script template

```javascript
module.exports = {
	'Page title is correct': function (test) {
  		test
    		.open('http://google.com')
    		.assert.title().is('Google', 'It has title')
    		.done();
	}
};
```

## Actions

[.query/$(selector)](http://dalekjs.com/docs/actions.html#meth-query) - Specifies a selector once for multiple actions or assertions on the same element(s)

[.end()](http://dalekjs.com/docs/assertions.html#meth-end) - Terminates a query statement

[.toFrame(selector)](http://dalekjs.com/docs/actions.html#meth-toFrame) - Switches to an iframe context

[.toParent()](http://dalekjs.com/docs/actions.html#meth-toParent) - Switches back to the parent page context

[.toWindow(id)](http://dalekjs.com/docs/actions.html#meth-toWindow) - Switches to a different window context

[.toParentWindow()](http://dalekjs.com/docs/actions.html#meth-toParentWindow) - Switches back to the parent window context

[.screenshot(path)](http://dalekjs.com/docs/actions.html#meth-screenshot) - Take a screenshot of the current page

[.open(url)](http://dalekjs.com/docs/actions.html#meth-open) - Performs an HTTP request for opening a given location

[.wait(time)](http://dalekjs.com/docs/actions.html#meth-wait) - Pause steps suite execution for a given amount of time (default time: 5000ms)

[.waitFor(function)](http://dalekjs.com/docs/actions.html#meth-waitFor) - Waits until a function returns true to process any next step (default time: 500ms)

[.waitForElement(selector, time)](http://dalekjs.com/docs/actions.html#meth-waitForElement) - Waits until an element exists in remote DOM (default time: 5000ms)

[.reload()](http://dalekjs.com/docs/actions.html#meth-reload) - Reloads current page location

[.forward()](http://dalekjs.com/docs/actions.html#meth-forward) - Moves a step forward in browser's history

[.back()](http://dalekjs.com/docs/actions.html#meth-back) - Moves back a step in browser's history

[.click(selector)](http://dalekjs.com/docs/actions.html#meth-click) - Performs a click on the element matching the provided selector expression

[.submit(selector)](http://dalekjs.com/docs/actions.html#meth-submit)- Submits a form

[.type(selector, text)](http://dalekjs.com/docs/actions.html#meth-type) - Types a text into an input field or text area

[.sendKeys(selector, codes)](http://dalekjs.com/docs/actions.html#meth-sendKeys) - This acts just like .type(), just for non-input elements, such as: tab, enter etc.

[.setCookie(name, value)](http://dalekjs.com/docs/actions.html#meth-setCookie) - Sets a cookie

[.setValue(selector, value)](http://dalekjs.com/docs/actions.html#meth-setValue) - Fills the fields of a form with given values

[.answer(text)](http://dalekjs.com/docs/actions.html#meth-answer) - Types a text into the text input field of a prompt dialog

[.execute(function)](http://dalekjs.com/docs/actions.html#meth-execute) - Executes a JavaScript function within the browser context

[.accept()](http://dalekjs.com/docs/actions.html#meth-accept) - Accepts an alert/prompt/confirm dialog

[.dismiss()](http://dalekjs.com/docs/actions.html#meth-dismiss) - Dismisses an prompt/confirm dialog

[.resize({width:, height:})](http://dalekjs.com/docs/actions.html#meth-resize) - Resizes the browser window to a set of given dimensions (in px)

[.maximize()](http://dalekjs.com/docs/actions.html#meth-maximize) - Maximizes the browser window

[.log.dom(selector)](http://dalekjs.com/docs/actions.html#meth-log.dom) - Logs a part of the remote dom

[.log.message(text)](http://dalekjs.com/docs/actions.html#meth-log.message) - Logs a user defined message

## Assertions

[.chain()](http://dalekjs.com/docs/assertions.html#meth-chain) - Specifies an assertion once for multiple checks

[.end()](http://dalekjs.com/docs/assertions.html#meth-end) - Terminates an assertion chain

[.numberOfElements(selector, n, output)](http://dalekjs.com/docs/assertions.html#meth-numberOfElements)\*\* - Asserts that a given element appears n times on the page

[.numberOfVisibleElements(selector, n, output)](http://dalekjs.com/docs/assertions.html#meth-numberOfVisibleElements)\*\* - Asserts that a given element is visible n times on the page

[.val(selector, value)](http://dalekjs.com/docs/assertions.html#meth-val)\* - Asserts that a given form field has the provided value

[.css(selector, property, value)](http://dalekjs.com/docs/assertions.html#meth-css) - Checks the computed style

[.width(selector, width)](http://dalekjs.com/docs/assertions.html#meth-width)\*\* - Checks the actual width of an element

[.height(selector, width)](http://dalekjs.com/docs/assertions.html#meth-height)\*\* - Checks the actual height of an element

[.selected(selector)](http://dalekjs.com/docs/assertions.html#meth-selected) - Determine if an element, or a :checkbox or :radio elements is currently selected

[.notSelected(selector)](http://dalekjs.com/docs/assertions.html#meth-notSelected) - Determine if an  element, or a :checkbox or :radio elements is currently not selected
                                                                                                     
[.enabled(selector, message)](http://dalekjs.com/docs/assertions.html#meth-enabled) - Determine if an element is currently enabled

[.disabled(selector, message)](http://dalekjs.com/docs/assertions.html#meth-disabled) - Determine if an element is currently disabled

[.cookie(name, value)](http://dalekjs.com/docs/assertions.html#meth-cookie) - Checks the contents of a cookie

[.exists(selector)](http://dalekjs.com/docs/assertions.html#meth-exists) - Asserts that an element exists in remote DOM environment

[.doesntExist(selector)](http://dalekjs.com/docs/assertions.html#meth-doesntExist) - Asserts that an element doesn't exist in remote DOM environment

[.notVisible(selector, message)](http://dalekjs.com/docs/assertions.html#meth-notVisible) - Asserts that an element is not visible

[.visible(selector, message)](http://dalekjs.com/docs/assertions.html#meth-visible) - Asserts that an element is visible

[.doesntHaveText(selector, text, message)](http://dalekjs.com/docs/assertions.html#meth-doesntHaveText) - Asserts that given text does not exist in the provided selector

[.dialogDoesntHaveText(text)](http://dalekjs.com/docs/assertions.html#meth-dialogDoesntHaveText) - Asserts that given text does not exist in the current alert/prompt/confirm dialog

[.text(selector, text, message)](http://dalekjs.com/docs/assertions.html#meth-text)\* - Asserts that given text does exist in the provided selector

[.dialogText(text)](http://dalekjs.com/docs/assertions.html#meth-dialogText)\* - Asserts that given alertText does exist in the provided alert/confirm or prompt dialog

[.title(text, message)](http://dalekjs.com/docs/assertions.html#meth-title)\* - Asserts that the page title is as expected

[.doesntHaveTitle(text, message)](http://dalekjs.com/docs/assertions.html#meth-doesntHaveTitle) - Asserts that given title does not match the given expectations

[.url(url, message)](http://dalekjs.com/docs/assertions.html#meth-url)\* - Asserts that the page's url is as expected

[.doesntHaveUrl(url, message)](http://dalekjs.com/docs/assertions.html#meth-doesntHaveUrl) - Asserts that the pages URL does not match the expectation

[.attr(selector, attribute, value)](http://dalekjs.com/docs/assertions.html#meth-attr)\* - Asserts that an elements attribute is as expected

## Assertions - Syntactic Sugar

### Textual assertions \*

.is(value, message) - Asserts that a given test on the page equals to a given value

.is.not(value, message) - Asserts that a given test on the page doesn't equal to a given value

.to.contain(value)- Asserts that a given test on the page contains a given value

### Numerical assertions \*\*

.is(n, message) - Asserts that a given element appears n times on the page

.is.between([m-n], message)- Asserts that a given element appears m-n times on the page

.is.gt(n, message)- Asserts that a given element appears more than n times on the page

.is.gte(n, message)- Asserts that a given element appears at least n times on the page

.is.lt(n, message)- Asserts that a given element appears less than n times on the page

.is.lte(n, message)- Asserts that a given element appears no more than n times on the page

.is.not(n, message)- Asserts that a given element not appears n times on the page

### Screenshots Path Variables

:browser- The browser name (e.g. 'Chrome', 'Safari', 'Firefox', etc.)

:version- The browser version (e.g. '100', '2311\_5', etc.)

:os- The operating system (e.g.OSX,Windows,Linux)

:osVersion- The operating system version (e.gXP,7,10\_8, etc.)

:viewport- The current viewport in pixels (e.g.w1024\_h768)

:timestamp- UNIX like timestapm (e.g.637657345)

:date- Current date in format MMDDYYYY (e.g.12\_24\_2013)

:datetime- Current datetime in format MMDDYYYYHHmm\_ss (e.g.12\_24\_2013\_14\_55\_23) 