# REGEX
Notes on REGEX with its application in python and git-ci.yml etc.

1. [a-m] <br />
   txt = "The rain in Spain" <br /> 
   import re <br />
   re.findall("[a-m]", txt) <br />
   
   - ['h', 'e', 'a', 'i', 'i', 'a', 'i']
   
2. '*'	- Zero or more occurrences <br />
   txt = "hello planet" <br />
   import re <br />
   x = re.findall("he.*o", txt) <br />
   
   NOTE: here we used a DOT alongwith a STAR -> '.*' -> basically DOT represents to search the character
  
3. ^	Starts with <br />
   txt = "hello planet" <br />
   x = re.findall("^hello", txt) <br />
   Yes, the string starts with 'hello'
   
4. $	Ends with   
   txt = "hello planet" <br />
   x = re.findall("planet$", txt) <br />
   Yes, ends with starts with 'planet'
   
5. '*'	Zero or more occurrences  -> "he.*o" <br />
   '+'  One or more occurrences   -> "he.+o" <br />
   '?'  ZERO or ONE occurrences   -> "he.?o" <br />
   {}   Exactly the specified number of occurrences -> "he.{2}o" <br /> <br />
   
   **NOTE: you have used a DOT '.' in all the above examples because DOT REPRESENTS any characters**
   
   
6. "\d"	Returns a match where the string contains digits (numbers from 0-9)  <br />
   txt = "The rain in Spain" <br />
   import re <br />
   x = re.findall("\d", txt) <br /> <br />
   
   NO MATCH

## References:
- https://www.w3schools.com/python/python_regex.asp
- https://ruby-doc.org/core-3.1.2/Regexp.html
