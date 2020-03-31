# go-gedcom555

A stab at implementing GEDCOM version 5.5.5.

GEDCOM is the standard format for genealogical files, but it has not been officially updated in ages (since "GEDCOM 5.5.1 beta") and it has some problems with representing a full range of genealogical data. There are currently two efforts to update the standard: one is known as GEDCOM 5.5.5 and the other is known as GEDCOM X.

GEDCOM X does not appear to be seeking compatibility and upgradability from GEDCOM 5.5.1, and its current implementation is written in Java, so it can be ignored. GEDCOM 5.5.5 on the other hand is highly compatible with (and pugradable from) 5.5.1, so it is worth pursuing.

Currently there are two Golang codebases addressing GEDCOM.

