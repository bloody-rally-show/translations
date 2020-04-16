# Bloody Rally Show Translations

Want to contribute a translation for your own language, or maybe fix an issue?
Make a Pull Request on GitHub: https://github.com/bloody-rally-show/translations

Before considering contributing a translation, please check for open pull requests
and if there is no folder already reserved to a language!

## Generic structure

Root Translations folder contains subfolders with specific languages. Those
language folders should be named after the properties of 
[Unity.SystemLanguage](https://docs.unity3d.com/ScriptReference/SystemLanguage.html)
(case sensitive).

English translation is default, and all missing keys will go to it as a fallback.
Main translation file has to be named in same way as the language folder, so for 
English it is English/English.csv, for Spanish it would be Spanish/Spanish.csv

Please use a text editor that supports UNIX new lines, if you open translation
files with Notepad, you may see all the words go in one line.

## Files

  * Language.csv - will be named English.csv or Spanish.csv, depending on the language.
    This is the meat of the game, containing almost everything. Format is similar to CSV,
    but it splits every line into key and value using just the first comma, so you can 
    have as many commas in the translation as you want, no need to escape or put anything into quotes.
    It is recommended to copy the English.csv and modify it without even changing the line order,
    without deleting comments or adding blank lines, so when anything changes, it will be
    easy to jump to the exact line and add something from English.csv
  * Appologies.txt - contains a list of short phrases that show up in speech bubbles after 
    racers hit each other or hit a pedestrian. Not necessarily apologetic phrases. The list 
    can have different amount of phrases for different languages. One phrase per line.
  * CurseAdjectives.txt - contains a list of adjectives that are usually combined with some noun
    when generating procedural dialogues. Can often be combined with something from the list of 
    insults (i.e. "damn hipsters"). Can have different amount of words for different languages.
    One word per line.
  * CurseAdverbs.txt - same as curse adjectives, but goes before a verb. Rarely used.
    Example "You are going to *friggin* die". Can have different amount of words for 
    different languages. One word per line.
  * Curses.txt - list of generic curses, that can show up in speech bubbles for racers
    and pedestrians, also used in some dialogues. Can have different amount of words
    for different languages, and can be very national and local. One curse per line.
  * Insults.txt - list of random insults that are used in procedurally generated dialogues. 
    Singular nouns. Don't go too offensive or crude, has to be subtle and on the light side.
    Can have different count for different languages, and can be very local. One insult per line.
  * InsultsPlural.txt - basically a plural versions of insults from Insults.txt
  * ItemsSlippery.txt - list of funny items with fluid / slippery properties, that
    will be used in dialogue generation. Something you can spill or rub on surfaces to make
    them slippery. Can be quite reguinal and locally specific too. Should not be single words.
    One item per line. Can have different count of items for each language.
  * ItemsSolid.txt - list of funny items with solid properties, that are not fluids, but still
    squishy or soft enough to be jammed into an exhaust pipe or stuffed into a helmet.
    Used in generating funny dialogues. Can be quite reguinal and locally specific too. 
    Should not be single words. One item per line. Can have different count of items for each language.
  * Tips.txt - list of random lines with game facts, tips and random jokes that appear on loading
    screens. Should most likely be translated as as, and maybe spiced a bit with something regional.
    One tip per line. Can have different count of items
  * Generation - contents of this folder are used to generate racer names and 
    random track / car / campaign names. Doesn't have to be translated, unless you want to make
    your local version 100% authentic.
