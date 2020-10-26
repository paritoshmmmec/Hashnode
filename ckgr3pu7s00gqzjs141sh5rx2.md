## Importance of Naming

Naming is essentials to programming. Names define ***identity *** of an object, variable, method or components, etc. 
A wrong/incorrect identity can lead to a wrong interpretation of the software component. This also can frustrate developers.

If a method is named `StartHeater` which carries the responsibility of starting the heater. Now assume if this method also asks for an additional parameter to increase the temp by x amount. Now identity/naming of this method has been lost. Ideally, This should be named now `StartHeaterAndIncreaseTemp` or should be broken down into two methods. 

Good naming can also generate new ideas e.g. if a component is named `EventStore`, a new developer in the team can guess without reading the source code of this component as the name is defining its identity. They also can interpret that this component might have a method which will store event or append events. On the contrary, if you see a component like `util` the same developer is going to make mistake. They are going to put anything inside util.


In nutshell, Think a bit more about naming stuff. Future developer will thank you.

PS: `util` is not a bad choice in some part of software.