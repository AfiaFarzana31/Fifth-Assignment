1. What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?

-->getElementById("id") finds one element by its unique ID.
-->getElementsByClassName("class") finds all elements with that class (gives a live HTMLCollection).
-->querySelector("selector") finds the first element that matches a CSS selector.
-->querySelectorAll("selector") finds all matching elements (returns a static NodeList).

2. How do you **create and insert a new element into the DOM**?

let el = document.createElement("p");  
el.textContent = "Hi there!";  
document.body.appendChild(el);

3. What is **Event Bubbling** and how does it work?

When an event happens (like a click), it starts at the target element and then bubbles up through its parent elements until it reaches the top (document).

4. What is **Event Delegation** in JavaScript? Why is it useful?

Event delegation means instead of adding a listener to many child elements, we add it once to the parent and catch events as they bubble up.
It is useful because it saves memory, works for dynamically added elements, and keeps code clean.

5. What is the difference between **preventDefault() and stopPropagation()** methods?

preventDefault() stops the browser’s default action (like a form submission or link navigation).
stopPropagation() stops the event from bubbling up to parent elements.
