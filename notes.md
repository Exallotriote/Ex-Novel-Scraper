### TO DO:
- [ ] Make it possible to download as an epub
	- Im thinking of having each chapter be recorded in a different key in local storage
- Fix chapters getting cut off bc of the size limit
	- no idea how to fix this yet. might have to just accept this as a limitation.
- [ ] so the data storage has a size limit right? what if when it reaches that file size limit i just delete the variable, then run the script again where it left off. so if it stopped at chapter 724 i can just delete the data storage and then run the script again
---
- Basic logic goes:
	- data variable gets a value from data storage. if data storage doesnt have anything, then data variable will become an empty string.
	- chapter content string gets added to data variable string. so
		- if E doesnt exist, then the variable's value becomes F
		- if E does exist then the variable's value becomes EF
		- istg if i still forget this i'll bang my head on wall
	- data storage is now equal to data variable
	- gets the next chapter link and goes to it
- If the stuff above is in a userscript then it will continously loop.
- as of now, it can only record a max file size of 343 kb, which is approximately 720 chapters.