========
Troubleshooting
========

Most of the errors you mentioned before are fixed, but there are some important points to remark:

- When the asignee is "nobody@mozilla.org" doesn't mean that the user isn't logged in, but that the bug hasn't been assigned to anyone. (When isn't logged in it says "nobody", you can check that https://bugzilla.mozilla.org/show_bug.cgi?id=1130155 logged in)

- The extraction of the profiles information fields are complicated to do since the website all the information with a table and for web scrapping a better structure with name of classes and id's on every HTML is needed. I'm facing this problem with a different approach, but for now those are the only fields that I can get.

- The method of the library that I'm using only let's me to get one CC email of the list, for this I need to switch the library for XML that I'm using but that might mean major changes on the code.

- The complete extraction of the data takes about 30 min for every project inside Mozilla, the data set I sent you early was just an example. (You can run it on your own with new version that I pushed).


With the new version of the script that I have uploaded, Parley must be able to make tests, although he mentioned errors occurred during the run of my script, in case any of this problems happen again I'll be checking the Node.js project that I wrote for testing purposes


Greetings. Diego.
