WWW
===

World With Words Scripts and Server Side 

A conceptual summaruy of Cues and Words can be found here
:http://slid.es/pronabpal/introducing-dwis

A demonstration of working DWIS.js is found here
: https://s3-us-west-2.amazonaws.com/onlywords/myCuesV0.html

The Cues are words as we use them . the main function is dwis.js library is the placeCue() function
which creates Cues.
A word created as Cue must have an entry as metaWords which is also maintained 
by dwis.js

Just like a prompter prompts a word to remind a performer a huge bunch of actions during a performance 

so our Cue is basicaly a collection of other words as in a bag of words. 
This bag of words however creates an illusion that the Cue is a parent of the words in the bag which it is not.

Howver this illusion works for us because this way Cue can work both as a Scope of words to come or a

flow of other Cue words to come , because each word is also a Cue.
I believe the concept of Cue is a powerful one to set  the communication latencies in small device and server 
communication in a meaningful fashion.
However there is plenty of things to be done including starting to code through Cues rather than just any object.

The concept is more important and that is the reason I am placing the JavaScript in the open so that any one can develop the concepts in his /her own way.
Please feel free to fork this.
I can be reached @: palpronab@gmail.com
Following is a quick tutorial for DWIS.js:


after down loading dwisV0.js   file  include the following in your html 
<script   src="dwisV0.js"> </script>
To instantiate a WWW object :
 { var W = new WWW(); }
To create a Word :
W.placeCue("w1") ;
w1 is added to the metaWords 
first time you introduce the word ; 
To place w1 in a cue word w2 :
W.placeCue("w1","w2");
Things to Note:

when you add a word , the spaces are replaced 
by a single "_" ; 
The word is added to a root named "root";
so the word created will be 'root.w1',
however the metaWord will be just 'w1'
however you can change the root
 by supplying the  name at time 
of construction :
var W = WWW("DrJones"); in this case W.placeCue("w1")  shall produce the Cue "DrJones.w1"

enjoy!
any questions :palpronab@gmailcom



