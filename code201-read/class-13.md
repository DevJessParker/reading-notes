# Local Storage

### Downside to Cookies

- Stores a small amount of data, but can slow down a web application

### History of Local Storage 

- When Microsoft created Internet Explorer, they created a behavior called userData. This stored 64 KB of data.

- AMASS (AJAX Massive Storage System): developed by Brad Neuberg and served as a link between JavaScript and Flash.

- AMASS became dojox.stored

- Gears: API that links to SQLite database. Created by Google


### HTML5 Storage

- Also known as Web Storage, Local Storage, or DOM Storage.

-Data is not sent to remote server.

- Created with the localStorage object.

- Modernizr.localstorage is a shortcut for a function that checks for local storage support in the browser.

- Limited to 5 MB and cannot ask for more.

- Data is stored as strings.