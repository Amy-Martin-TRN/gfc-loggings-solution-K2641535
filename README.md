Changelog

MyGame.cpp
Line 51 to 64: added obstacle interactions
L196 to 219: added new level layout
L307: specified that the logging must also NOT be a ghostling
L319 to 330: added new interaction - while GHOST is active, clicking a ghostling will execute Explode() function

MyObjects.cpp
L56: added new state "walk", which is used in obstacle interactions
L103+111: remove "walk" state from dropping/falling loggings
L113: moved x co-ordinate for dropping loggings by +20 for improved visual consistency when a falling logging hits a wall
L161: specified the logging must not be a ghostling
L167-171: added new outcome to Explode() function - when a ghostling calls this function, it will NOT explode, but instead become a normal logging (used in L319-330 of MyGame)
