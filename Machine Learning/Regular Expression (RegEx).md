

- Support differs in each regex engine
- Implementations may differ of the same engine

POSIX Standard Regexes:
- Basic Regular Expressions (BRE)
- Extended Regular Expressions (ERE)



ERE:

- . --> matches 1 characters
- [] --> character sets
- \ --> Escape single characters
- () --> Pattern Grouping
- | --> Alteration
- * + {} --> repetition operators
- ^abc --> leading anchor
- abc$ --> trailing anchor
- [^abc] --> negates pattern


Occurences:
. --> one character
.? --> zero or one character
.+ --> one or more occurrences
.* --> zero or more occurrences
.{3} --> three occurrences
.{3,} --> three or more occurrences
.{,3} --> zero to three occurrences
.{1,3} --> one to three occurrences