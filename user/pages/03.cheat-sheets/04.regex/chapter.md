---
title: Regex
---

#####Special Characters in Regular Expressions & their meanings

| Character | Meaning   | Example   |
|
| *         | Match **zero, one or more** of the previous| Ah* matches "Ahhhhh" or "A"|
| ?         | Match **zero or one** of the previous| Ah? matches "Al" or "Ah" |
| +         | Match **one or more** of the previous| Ah+ matches "Ah" or "Ahhh" but not "A"|
| \         | Used to **escape** a special character| Hungry\? matches "Hungry?"|
| .         | Wildcard character, matches **any** character| do.* matches "dog", "door", "dot", etc.|
| ( )       | **Group** characters| See example for &#124;|
| [ ]       | Matches a **range** of characters| [cbf]ar matches "car", "bar", or "far",  [0-9]+ matches any positive integer, [a-zA-Z] matches ascii letters a-z (uppercase and lower case), [^0-9] matches any character not 0-9.|
| &#124;       | Matches previous **OR** next character/group| (Mon)&#124;(Tues)day matches "Monday" or "Tuesday"|
| { }       | Matches a specified **number of occurrences** of the previous| [0-9]{3} matches "315" but not "31"&#124; [0-9]{2,4} matches "12", "123", and "1234"&#124; [0-9]{2,} matches "1234567..." |
| ^         | **Beginning** of a string. Or within a character range [] negation.| ^http matches strings that begin with http, such as a url.&#124; [^0-9] matches any character not 0-9.|
| $         | **End** of a string.| ing$ matches "exciting" but not "ingenious"|


