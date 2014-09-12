ReactWebSocket
==============
Testing HTML5 WebSockets and React Library

http://facebook.github.io/react/
http://www.websocket.org/index.html

First Trying the Echo Test
http://www.websocket.org/echo.html

Next, I'm trying to combine the TODO LIST
http://facebook.github.io/react/index.html

===============
Goal
===============

Main goal is to combine this echo test with the TODO list, so that HTML5 WebSockets are used as well as React.js
Such that there will be one box for sent and another for recieved messages.

===============
Errors
===============
One error I encountered is that the React.renderComponent function must be executed only after the DOM component, otherwise an error will be thrown.

The other significant error I encountered was dealing with the Javascript Object heirarchy, particulary in the testwebSocket function. I had to learn of the trick of doing var self = this; because if I used this.onOpen(evt), it would mean using something equivalent to websocket.onOpen which was undefined.
http://stackoverflow.com/questions/10175853/how-to-assign-functions-in-javascript

==============
Final Problems
==============
I did not have enough time to deal with the problem of websockets.close() refreshing the page, and having the complete disconnected/connected functionality of the websocket.org echo page.
