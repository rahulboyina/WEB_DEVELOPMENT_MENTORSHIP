DOM (Document Object Model) manipulation in JavaScript allows you to interact with and change the structure, style, and content of a webpage.

Here are some common DOM manipulation techniques:

1. **Selecting Elements**:

   - `getElementById()`: Gets an element by its ID.
   ```javascript
   let element = document.getElementById('myElement');
   ```

   - `getElementsByClassName()`: Gets elements by their class name.
   ```javascript
   let elements = document.getElementsByClassName('myClass');
   ```

   - `getElementsByTagName()`: Gets elements by their tag name.
   ```javascript
   let elements = document.getElementsByTagName('div');
   ```

   - `querySelector()`: Gets the first element that matches a CSS selector.
   ```javascript
   let element = document.querySelector('.myClass');
   ```

   - `querySelectorAll()`: Gets all elements that match a CSS selector.
   ```javascript
   let elements = document.querySelectorAll('.myClass');
   ```

2. **Manipulating Element Properties**:

   - `element.textContent`: Sets or gets the text content of an element.
   ```javascript
   element.textContent = 'New Text';
   ```

   - `element.innerHTML`: Sets or gets the HTML content of an element.
   ```javascript
   element.innerHTML = '<strong>Bold Text</strong>';
   ```

   - `element.style.property`: Changes the CSS style of an element.
   ```javascript
   element.style.color = 'blue';
   ```

3. **Creating New Elements**:

   - `document.createElement()`: Creates a new element.
   ```javascript
   let newElement = document.createElement('div');
   ```

   - `element.appendChild()`: Appends a child element to a parent element.
   ```javascript
   parentElement.appendChild(newElement);
   ```

4. **Removing Elements**:

   - `element.remove()`: Removes an element from the DOM.
   ```javascript
   element.remove();
   ```

5. **Adding and Removing Classes**:

   - `element.classList.add()`: Adds a class to an element.
   ```javascript
   element.classList.add('newClass');
   ```

   - `element.classList.remove()`: Removes a class from an element.
   ```javascript
   element.classList.remove('oldClass');
   ```

6. **Event Handling**:

   - Adding an event listener to an element.
   ```javascript
   element.addEventListener('click', function() {
     // Your code here
   });
   ```

   - Removing an event listener from an element.
   ```javascript
   element.removeEventListener('click', functionName);
   ```

7. **Traversing the DOM**:

   - Moving up the DOM tree.
   ```javascript
   let parentElement = element.parentNode;
   ```

   - Moving down the DOM tree.
   ```javascript
   let childElement = element.children[0];
   ```

8. **Modifying Attributes**:

   - Getting an attribute's value.
   ```javascript
   let value = element.getAttribute('src');
   ```

   - Setting an attribute's value.
   ```javascript
   element.setAttribute('src', 'newImage.jpg');
   ```

Remember to always consider performance and efficiency when manipulating the DOM, especially for complex web applications. Batch your changes where possible, and consider using techniques like event delegation for improved performance.
