# go-gedcom555

go-gedcom555 takes a stab at implementing GEDCOM version 5.5.5.

*GEDCOM* is the generally accepted standard format for genealogical files. 
However, it has not been officially updated in ages (not since "GEDCOM 
5.5.1 beta") and it has some problems with representing a full range of 
genealogical data. 

There are currently two efforts to update the standard: 
one is known as GEDCOM 5.5.5 and the other is known as GEDCOM X.

*GEDCOM X* has several issues (IMHO). There hasn't been (AFAICT) much 
activity on it for years. There is no mention of compatibility with 
or upgradability from GEDCOM 5.5.1. Its only current implementation 
is written in Java. So, let's ignore it, at least for now. 

*GEDCOM 5.5.5* on the other hand is highly compatible with 
(and upgradable from) 5.5.1, so this is worth pursuing.

Currently there are two Golang codebases addressing GEDCOM.

