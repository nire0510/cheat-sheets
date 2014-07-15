# [DalekJS](http://dalekjs.com/) Cheat Sheet v0.0.8

# Actions

[.query/$(selector)](http://dalekjs.com/docs/actions.html#meth-query) - Specifies a selector once for multiple actions or assertions on the same element(s)

.end() - Terminates a query statement

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

# Assertions

[.chain()](http://dalekjs.com/docs/assertions.html#meth-chain) - Specifies an assertion once for multiple checks

[.end()](http://dalekjs.com/docs/assertions.html#meth-end) - Terminates an assertion chain

[.numberOfElements(selector, n, output)](http://dalekjs.com/docs/assertions.html#meth-numberOfElements)\*\* - Asserts that a given element appears n times on the page

[.numberOfVisibleElements(selector, n, output)](http://dalekjs.com/docs/assertions.html#meth-numberOfVisibleElements)\*\* - Asserts that a given element is visible n times on the page

[.val(selector, value)](http://dalekjs.com/docs/assertions.html#meth-val)\* - Asserts that a given form field has the provided value

[.css(selector, property, value)](http://dalekjs.com/docs/assertions.html#meth-css) - Checks the computed style

[.width(selector, width)](http://dalekjs.com/docs/assertions.html#meth-width)\*\* - Checks the actual width of an element

[.height(selector, width)](http://dalekjs.com/docs/assertions.html#meth-height)\*\* - Checks the actual height of an element

[.selected(selector)](http://dalekjs.com/docs/assertions.html#meth-selected) - Determine if an 