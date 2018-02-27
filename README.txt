

	+===============================================+
	|		THANK YOU SO MUCH !!!		|
	|						|
	|	Translating is a big job, and we're	|
	|	very grateful for your help.		|
	|						|
	+===============================================+



		-=-=-=-= HOW TO DO IT =-=-=-=-=-

There are over 40,000 words to translate,
fortunately the process is rather simple.

In this localisation kit you will find several files:

English_dialog_messages.txt
English_injury_messages.txt
English_UI_messages.txt

Etc etc..

If you open a file, you will notice multiple lines
Separated by the '%' symbol.
	- !!! DO NOT REMOVE OR CHANGE THESE % !!!
Everything between the '%' symbol is text that needs to be
Translated. If you need to use a '%' symbol, use '$' instead,
It will be replaced in game as '%'.

e.g. "Hello.%" would simply be replaced as "Bonjour.%"
Always leave the '%' symbol at the end of the segment.
And "Gain 10$ more.%" would be seen in game as "Gain 10% more."

You may find a few duplicated messages, please copy and paste the translation,
Or treat it like a normal line.
	- !!! DO NOT DELETE OR REMOVE DUPLICATE LINES !!! -
(There should only be a handful, and close to each other.)

If you find something that looks like: [MappedKey:Submit] DO NOT REMOVE IT.
This will automatically be replaced with the keybinding text. Instead, move
The [MappedKey] to where you want the keybinding to show.

e.g. "Press the [MappedKey:Attack] button" could be moved to read
"The [MappedKey:Attack] button is for attacking" etc. which might end up being:
"The Right Trigger button is for attacking."

Once you have translated all of the text in a .txt files, change the
Name from "English_" to the new language.

e.g. Instead of "English_UI_messages.txt" you might change it
to read "French_UI_messages.txt"



		-=-=-=-= ITEM GENERATION =-=-=-=-=-

There are four separate files for item name generation:
	English_item_prefixes.txt
	English_item_materials.txt
	English_item_types.txt
	English_item_suffixes.txt
When an item is generated in game, it will be created in the order:
	prefix -> material -> type -> joiner -> suffix
e.g. "Cursed Leather Cap of the monkey clan"

You can change the order of the item generation in English_item_order.txt
DO NOT USE CAPITAL LETTERS and DO NOT USE SPACES.
e.g. prefix+type+material+joiner+suffix

In suffixes you will also find two extra references, (" of the" and " of")
(" Of the") will be used for the first 12 suffixes, and (" of") for the remaining 24.



		-=-=-=-= NAME GENERATION =-=-=-=-=-

There are also other names that are generated, companions, and bounties. However, they are simply: name+suffix.

There are a lot of names or descriptions which may not translate, you're free to come up with your own suitable compromise.

If for translation purposes you need it to be suffix+name, simply swap the lines with one another.

e.g instead of:
bob%
fred%
bill%
The dumb%
The silly%
The idiot%

You can re-order them like:

The dumb%
The silly%
The idiot%
bob%
fred%
bill%

(Make sure you re-order ALL names with ALL suffixes. And that they are of equal number of lines. Do not swap 5 suffixes with 10 names, for example. It must be 1:1)





















