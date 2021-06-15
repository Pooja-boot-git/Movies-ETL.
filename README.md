# Movies-ETL.
Amazing Prime video would like to know which low budget movies are being released and would become popular so they can buy streaming rights for those movies. In order to do so, they are conducting a hackathon and the participants are required to predict which will be the popular movies. Participants are being provided clean data extracted from two different sources (Wikipedia and Movie Lens ratings data) and we are going to transform and club it together using the power of Python and regular expressions. The transformed data will then be stored in SQL database POSTGRES. 


# REGULAR EXPRESSIONS BASICS

.	Any character except newline
a	The character a
ab	The string ab
a|b	a or b
a*	0 or more a's
\	Escapes a special character
Regular Expression Quantifiers
*	0 or more
+	1 or more
?	0 or 1
{2}	Exactly 2
{2, 5}	Between 2 and 5
{2,}	2 or more
(,5}	Up to 5
Default is greedy. Append ? for reluctant.
Regular Expression Groups
(...)	Capturing group
(?P<Y>...)	Capturing group named Y
(?:...)	Non-capturing group
\Y	Match the Y'th captured group
(?P=Y)	Match the named group Y
(?#...)	Comment
Regular Expression Character Classes
[ab-d]	One character of: a, b, c, d
[^ab-d]	One character except: a, b, c, d
[\b]	Backspace character
\d	One digit
\D	One non-digit
\s	One whitespace
\S	One non-whitespace
\w	One word character
\W	One non-word character
Regular Expression Assertions
^	Start of string
\A	Start of string, ignores m flag
$	End of string
\Z	End of string, ignores m flag
\b	Word boundary
\B	Non-word boundary
(?=...)	Positive lookahead
(?!...)	Negative lookahead
(?<=...)	Positive lookbehind
(?<!...)	Negative lookbehind
(?()|)	Conditional
Regular Expression Flags
i	Ignore case
m	^ and $ match start and end of line
s	. matches newline as well
x	Allow spaces and comments
L	Locale character classes
u	Unicode character classes
(?iLmsux)	Set flags within regex
Regular Expression Special Characters
\n	Newline
\r	Carriage return
\t	Tab
\YYY	Octal character YYY
\xYY	Hexadecimal character YY
Regular Expression Replacement
\g<0>	Insert entire match
\g<Y>	Insert match Y (name or number)
\Y	Insert group numbered Y
