# worldarcheryapi
Notes on deconstructing the world archery results API (api.worldarchery.org)

Query format

Event data
https://api.worldarchery.org/?content=COM&Detailed=1&CompId=15914&RBP=All&v=3

Individual archer results
https://api.worldarchery.org/?content=QUAINDARROWS&CompId=15914&CatCode=CW&Id=14331&RBP=All&v=3

# content

_string_ 
Kind of request being made:

* COM - Competition information
* QUAINDARROWS - Qualifying Individual Arrows
* ...

# Detailed

_boolean_ Verbosity flag. 0 for false, 1 for true
Having it set to false returns data that would be needed for a summary-style view.

# CompId

_integer_ Competition ID

# CatCode

_integer_ Category Code

* CW - Compound Women
* CM - Compound Men
* RW - Compound Women
* RM - Compound Men
* ...

# RBP

_string_ Unknown at this stage...

# v

_integer_ Assumed to be API version number. 3 seems to be the defualt.

