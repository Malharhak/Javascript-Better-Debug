Javascript-Better-Debug
=======================

Better debugging for Javascript with tags

##Why :
To debug complex applications, you need some little things :
1. Tags to see what is logging
2. Some debug boolean to activate/unactivate levels of logging

##How to :

1. Insert the debug object in your code (this lib is require.js-friendly).
2. Change the config to enable/disable some things
		
		this.logs = true; // Classic logs
		this.warns = true; // Warns, they appear with a warning sign in chrome
		this.errors = true; // Red stuff. That's for bad stuff. Mostly.

3. Log things
	
		debug.log("tag", "stuff", [1, 2, 3], {"test" : "hi"});
		debug.warn("tag", "O HAI");
		debug.error("tag", "Look, I'm an error.");

##Other stuff :

If you don't put any tag, it will show as "[UNTAGGED] : "
I think there is some color stuff possible with the console. If anyone wants to add these features...