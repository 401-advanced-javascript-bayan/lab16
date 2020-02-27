# lab16
Links and Resources
repo
Build Status
Documentation
jsdoc
Modules
./index.js

./app.js

./events.js

./logger.js

./lib/read.js

./lib/uppercase.js

./lib/write.js

./index.js
Exported Values and Methods
This is the entry point of the application that accepts the application's command line arguments.

.src/app.js
Exported Values and Methods
alterFile(file) -> undefined
This function takes a filepath and uses the helper functions read, uppercase, and write to capitalize the letters in the file. It emits appropriate events in its try/catch block.
./events.js
Exported Values and Methods
This module instantiates an events listener.
./logger.js
Exported Values and Methods
This module provides event listeners and handling functions that log to the console.

handleRead(payload) -> log
handleWrite(payload) -> log
handleAlter(payload) -> log
handleUppercase() -> log
handleError(payload) -> log
./lib/read.js
Exported Values and Methods
This module reads a file and returns a Promise. It emits events as appropriate.

read(file) -> Promise -> buffer
./lib/uppercase.js
Exported Values and Methods
uppercase(data) -> modified data This module takes a readable buffer or other input, converts it to a string, and capitalizes its letters. It emits events as appropriate.
.//lib/write.js
Exported Values and Methods
write(file, text) -> Promise -> side effect This module reads a file and returns a Promise. It writes a file with the given text as a side effect. It emits events as appropriate.
UML 
![](https://www.researchgate.net/profile/Michel_Parent/publication/4180724/figure/fig1/AS:279963849773057@1443759991123/Event-system-UML-class-diagram-The-three-central-interfaces-that-define-the-event-model.png)