# Links re. GEDCOM 5.5.5 

This is just a link dump. Don't read too much into the 
links themselves or the order in which they are given.

[The latest version of GEDCOM is GEDCOM 5.5.5, released on 2 Oct 2019. It succeeds GEDCOM 5.5.1, released on 2 Oct 1999.](https://www.gedcom.org/)

_It is a deliberate feature of GEDCOM 5.5.5 that <br/> 
you can manually change the version number from 5.5.5 to 5.5.1, <br/>
thereby downgrading a GEDCOM 5.5.5 file to a GEDCOM 5.5.1 file, <br/>
so it can be imported by apps that do not support GEDCOM 5.5.5 yet._<br/>
_By the way, this feature works only in one direction; <br/>
you **can** **down**grade a 5.5.5 file to a 5.5.1 file by changing the version number, <br/> 
you can**not** **up**grade a 5.5.1 file to a 5.5.5 file by changing the version number, <br/>
because most 5.5.1 files simply aren't up to GEDCOM 5.5.5 standards._

The [GEDCOM 5.5.5 press release](https://www.gedcom.org/press/PRGEDCOM555.pdf) lists the improvements:
* All GEDCOM identifiers must be alphanumerical now
* Simplified GEDCOM grammar
* Clarification that tags are case-sensitive
* A well-defined version number format
* LF+CR is no longer a legal line terminator
* No CONC or CONT in GEDCOM header
* Unicode Byte Order Mark (BOM) is mandatory
* Clear, simple rules about whitespace
* Simple CONC & CONT rules

The page 
[Just a revision](https://www.tamurajones.net/GEDCOM555JustARevision.xhtml)
expands on this:
* Better, more accurate and more consistent terminology. 
* Many typos and minor specification errors, such as the maximum length of media file names, have been corrected. 
* Contradictions have been resolved, existing specifications has been clarified. 
* Obsolete, deprecated and superfluous stuff has been taken out. 
* Resolves conflicts between the specification and actual practice. 
* The grammar rules have been simplified and tightened. 
* The grammar clearly distinguishes between characters used for GEDCOM itself and those used for user text, such as names and notes. 
* Identifiers and escape sequences no longer allow almost any character, but demand alphanumeric characters instead. 
* _(Simplifications...)_
* Each GEDCOM 5.5.5 file is just one file, has just one GEDCOM version per file, just one line terminator per file, and just one encoding per file. 
* There is just one character set for GEDCOM 5.5.5, just one submitter per GEDCOM file, and just one place name format. 
* There is just one record for each thing, and just one record format for each record.
* Unicode only.
* Clear & simple CONC & CONT rules, using only one set of religious records for all religions.
* One multimedia record per file & one file per multimedia record.

# Online validation

* It is available [online](http://ged-inline.elasticbeanstalk.com/validate)
* Open source! [Java under MIT license](https://github.com/nigel-parker/gedinline)
* It has (or, had) [some problems](https://www.tamurajones.net/GEDCOMValidatorIdentifierHandling.xhtml)

# Implementation issues

* [Best practices](https://www.tamurajones.net/GEDCOMForm.xhtml)
* Not LINEAGE-LINKED but LINAGE-LINKED, LINEAGE_LINKED, Lineage - Linked
* Event GEDCOM never caught on, isn't widely supported, and is practically forgotten.
* If HEAD.GEDC.FORM.FORM is EVENT, issue an informational message, and continue processing as a LINEAGE-LINKED GEDCOM. Validating Event GEDCOM is an optional advanced feature, so it is okay to simply report errors for all unrecognised tags.
* The GRAMPS Wiki "GRAMPS and GEDCOM page" discusses GRAMPS XML that gets lost by GEDCOM.

