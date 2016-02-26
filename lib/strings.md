---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a series of characters contained within single or double quotation marks. In situations where the string contains an apostrophe (such as the phrase "I don't know") it can be helpful to use double quotation marks instead of single, to avoid truncating the string prematurely. Single quotation marks can be used in these cases, so long as the string contains a "\" before the problematic character.

# What are some examples of information that would be Strings as opposed to some other data type?

Anything that is best expressed in text format, such as names, quotes, or the body text of a webpage.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

You can use the str[index] method, where "str" is the string you want to use (in this case, `"Ada Lovelace"`), and "index" is an intiger equal to 1 less than the place of the character you're looking for. So, `"Ada Lovelace"`[5] would return " ", the 6th character in the string, and `"Ada Lovelace"`[7] would return "o", the 8th character. If the index is greater than the number of characters in the string, it will return "nil".

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes. The "-6th" character in a string is the character that is 6 places from the end. To find the -6th character, you use basically the same method as finding the 6th (positive) character in a string: `"Ada Lovelace"`[-6]. 

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

`"Sumeet Jain"`.gsub('e','!') will replace all of the instances of 'e' in the string `"Sumeet Jain"` with '!'. If 'sub' is used instead of 'gsub' as the method, it will only relplace the first occurence of 'e'.
