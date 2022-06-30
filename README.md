# Google Dino

This hack allows your dinosaur to become invincible, letting players continue the game without fear of being poked or pecked.

To hack the game, you’ll need to be on the “No Internet” screen, so go ahead and enter chrome://dino in the address bar. 

Once in the “Console” tab, paste the following command and then press the “Enter” key:
var original = Runner.prototype.gameOver

Next, enter this command:
Runner.prototype.gameOver = function (){}

As you can see, the dinosaur is unaffected by the cacti or flying creatures. Mission accomplished.

Now, let’s say you’ve been playing for 25 minutes and you want to stop the game and record your high score. You’ll need a way to end the game, which can no longer be done by running into a cactus.

Remember the first code we entered? That stored the normal gameOver function in the original variable. That means we can now execute this command to use the normal gameOver function:
Runner.prototype.gameOver = original

