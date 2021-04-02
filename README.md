# OpenCart-3 Electrozon Parser

License: GPLv3.

Parser:
+ Uploading a config.php file (database data)
+ Loading the parameter of the markup from the base, and the tables with charges (if any)
+ Creates a TEMP log to record events
+ Removal of categories that are disappeared from the base, and the goods too
+ Features - Uploading from the site
- price rounding up to 10 - over 1000
- Make Checking Tables Database on Goods for Errors
- If any records in the database lack, add (correct)
- Cleaning (checking) pictures, removal of non-pull
Parsit Sections:
+ Compare sections that are in the database with those in the file, if there are deleted - record in the log
+ Removes excluded
+ if the section is updated
+ if there is no section - create
+ Picture, if there is in the database, save
Parsit Products:
+ compares the goods - if some removed, writes in log
+ Removes excluded
+ if the goods are - update
+ if there is no product - create
+ save SEO categories
+ save CEO
+ When creating (updating) of goods: Create its parameters,
+ download the specification from its page,
+ Download pictures from his page.
+ write vendor / product manufacturer
+ The markup is determined from the table (if any), if not, is made from the default parameter
Setting up a parser in admin:
- checking the availability of a table in the database if not - create
- Make in the settings the form of extraction charges in the category
- Make a parser in classes, try to make a universal parser work scheme
- Checking DB
- reading log files 2018-12-06_12-34, reading current dates / time
- Definition of the range as passed
- If the term came out, run the parser
- output of information on the last log
- Create groups of categories for which the markup can be set
- Earls to work in categories - component parameters (extended form)
- Make a button - RESET, which clears the table and all files
- Custom parser parameters (view in its TODO code)
- Parasera parameters - in the settings, what to do with excluded goods (auto date?)

O-8V6Z2-D2

TODO.
- Supplier (electroson, cylinding) - can be held in the table of surcharges
- either set the identifier prefix (specified in SKU)
- Product Supplier - location,

V-BIND OR: - Binding to variables
V-IF Conditions (visibility) <span v-if = "SEEN">
V-for - cycles <li v-for = "TODO IN TODOS"> {{TODO.TEXT}}
V-on or @Click - Events
V-model - for forms binding
V-HTML - Substitutes Data Instead of {{}} <Span V-HTML = "RAWHTML"> </ SPAN>
  


