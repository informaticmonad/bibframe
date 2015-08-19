<!---

BIBFRAME Archive is a starting point for archival vocabularies using the 
http://bibfra.me model and profiles. It builds off of the BIBFRAME Lite vocabulary. 
It is framework conformant to BIBFRAME and . and where possible, link-compatible with the 
US Library of Congress's BIBFRAME vocabulary, http://bibframe.org/

BIBFRAME Rare is expressed using the Versa data model, which also
allows for full expression in RDF form.  This particular file is in
the Versa Literate syntax, based on the Markdown format
<https://daringfireball.net/projects/markdown/basics>.

The convention for expressing data models in Versa Literate has each
vocabulary item starting with a new header, A level 1 header for
resource classes and level 2 for properties.  Each has its ID as an
IRI reference (usually relative). Each is then described within its
section's unordered list, given a "label" (display label),
"description" (also for explanatory display), possibly "synonyms" (one
or more loose expression that the resource can be considered a synonym
for another). Resource classes may also have "properties"
(space-separated list of property IDs defined on the
resource). Properties may also have "value" (textual description of
the expected value of the property, perhaps as a relationship to
another resource, or as a data value).

You'll notice that BIBFRAME Archive terms use a humpCase/HumpCase convention,
which derives from BIBFRAME legacy.

-->

# @docheader

<!---

@base is the default base IRI, used e.g. for resource headers. It
would also be used for properties except that it is overridden by
@property-base

The meta-properties in this file are actually defined by the Versa
data model to support interpretation by Versa modeling tools

@resource-base is another possible override, for resource headers, but
not used here

-->

* @iri:
    * @base: http://bibfra.me/vocab/archive/
    * @property: http://bibfra.me/purl/versa/support
* title: BIBFRAME Archive vocabulary
* @interpretations:
    * scope: @resource

<!---
Extend BIBFRAME Lite Classess
--->

# <http://bibfra.me/vocab/lite/Work>
* properties:  

# <http://bibfra.me/vocab/lite/Instance>
* properties: 

# <http://bibfra.me/vocab/lite/Authority>

# <http://bibfra.me/vocab/lite/Person>
* properties: 

# <http://bibfra.me/vocab/lite/Organization>
* properties: 

# <http://bibfra.me/vocab/lite/Meeting>
* properties: 

# <http://bibfra.me/vocab/lite/Topic>
* properties: 

# <http://bibfra.me/vocab/lite/Form>
* properties: 

<!---

Class Refinements 
-->


# findingAid

* label: finding aid
* refines: <http://bibfra.me/vocab/lite/findingAid>
* synonyms: 
* description: A work with finding aid characteristics that describes archival collections to give the repository physical and intellectual control over the materials, and assist users in gaining access to and understanding the materials
* value: Literal
* properties: eadId 
* scope: <http://bibfra.me/vocab/archive>
* remark: 

<!---

Properties - [Terms below are mapped from Structural and Other Limited EAD Elements]

-->

## eadId

* label: EAD Identifier
* refines: <http://bibfra.me/vocab/lite/controlCode>
* synonyms: 
* description: Designates a unique code for a particular EAD finding aid document
* value: Literal
* scope: <http://bibfra.me/vocab/archive>
* remark: Equivalent to EAD ID <eadid>

<!---

List of EAD Elements:

<filedesc> – 
<titlestmt> – Title Statement
<titleproper> – Title Proper
<subtitle> – Subtitle
<author> – Author
<sponsor> – Sponsor
<editionstmt> – Edition Statement
<publicationstmt> – Publication Statement
<publisher> – Publisher
<seriesstmt> – Series Statement
<notestmt> – Note Statement
<profiledesc> – Profile Description
<creation> – Creation
<langusage> – Language Usage
<language> – Language
<descrules> – Descriptive Rules
<revisiondesc> – Revision Description
<change> – Change
<list> as used within <revisiondesc>
<frontmatter> – Front Matter
<div> – Text Division
<titlepage> – Title Page
<archdesc> – Archival Description
<did> – Descriptive Identification
<abstract> – Abstract
<langmaterial> – Language of the Material
<physdesc> – Physical Description
<dimensions> – Dimensions
<extent> – Extent
<physfacet> – Physical Facet
<physloc> – Physical Location
<repository> – Repository
<subarea> – Subordinate Area
<unitid> – ID of a Unit
<unittitle> – Title of a Unit
<unitdate> – Date of a Unit


Terms below are mapped from generic elements used within <archdesc>, <archdescgrp>, <c>/<c01> (through <c12>), and <descgrp>


<accessrestrict> – Conditions Governing Access
<accruals> – Accruals
<acqinfo> – Acquisition Information
<altformavail> – Alternative Form Available
<appraisal> – Appraisal Information
<arrangement> – Arrangement
<bibliography> – Bibliography
<bioghist> – Biography or History
<c> – Component (Unnumbered)
<c01> – Component (First Level) through Component (Twelfth Level(
<container> – Container
<controlaccess> – Controlled Access Headings
<custodhist> – Custodial History
<dao> – Digital Archival Object
<daodesc> – Digital Archival Object Description
<daogrp> – Digital Archival Object Group
<daoloc> – Digital Archival Object Location
<descgrp> – Description Group
<dsc> – Description of Subordinate Coordinates
<fileplan> – File Plan
<index> – Index
<indexentry> – Index Entry
<legalstatus> – Legal Status
<odd> – Other Descriptive Data
<originalsloc> – Location of Originals
<otherfindaid> – Other Finding Aid
<phystech> – Physical Characteristics and Technical Requirements
<prefercite> – Preferred Citation
<processinfo> – Processing Information
<relatedmaterial> – Related Material
<scopecontent> – Scope and Content
<separatedmaterial> – Separated Material
<userestrict> – Conditions Governing Use
Generic Elements

<abbr> – Abbreviation
<address> – Address
<addressline> – Address Line
<bibseries> – Bibliographic Series
<blockquote> – Blockquote
<chronitem> – Chronology List Item
<chronlist> – Chronology List
<corpname> – Corporate Name
<date> – Date
<defitem> – Definition List Item
<edition> – Edition
<emph> – Emphasis
<event> – Event
<eventgrp> – Event Group
<expan> – Expansion
<famname> – Family Name
<function> – Function
<genreform> – Genre/Physical Characteristic
<geogname> – Geographic Name
<head> – Heading
<head01> – First Heading
<head02> – Second Heading
<imprint> – Imprint
<item> – Item
<label> – Label
<lb /> – Line Break
<list> – List
<listhead> – List Heading
<materialspec> – Material Specific Details
<name> – Name
<namegrp> – Name Group
<note> – Note
<num> – Number
<occupation> – Occupation
<origination> – Origination
<p> – Paragraph
<persname> – Personal Name
<repository> – Repository
<subarea> – Subordinate Area
<subject> – Subject
<title> – Title
Table Elements

<table> – Table
<tgroup> – Table Group
<colspec> – Table Column Specification
<thead> – Table Head
<tbody> – Table Body
<row> – Table Row
<entry> – Table Entry


Terms below are mapped from EAD linking elements


<arc> – Arc
<archref> – Archival Reference
<bibref> – Bibliographic Reference
<dao> – Digital Archival Object
<daodesc> – Digital Archival Object Description
<daogrp> – Digital Archival Object Group
<daoloc> – Digital Archival Object Location
<extptr> – Extended Pointer
<extptrloc> – Extended Pointer Location
<extref> – Extended Reference
<extrefloc> – Extended Reference Location
<ptr> – Pointer
<ptrgrp> – Pointer Group
<ptrloc> – Pointer Location
<ref> – Reference
<refloc> – Reference Location/li>
<resource> – Resource
Other Elements

<eadgrp> – EAD Group
<archdescgrp> – Archival Description Group
<dscgrp> – Description of Subordinate Components Group
<runner> – Runner

-->

## titleProper

* label: title proper
* refines: <http://bibfra.me/vocab/lite/title>
* synonyms: 
* description: The proper title
* value: Literal
* scope: <http://bibfra.me/vocab/dcrmb>
* remark: Required element.

## datePublication

* label: date publication
* refines: <http://bibfra.me/vocab/lite/providerDate>
* description: The date of publication.
* value: Literal
* scope: <http://bibfra.me/vocab/dcrmb>
* remark: Required element. Recommended ISO 8601 date.

## signature

* label: signature
* refines: <http://bibfra.me/vocab/lite/note>
* description: Lists or summaries of signatures often printed at the end of early printed books.
* value: Literal
* scope: <http://bibfra.me/vocab/dcrmb>


<!---

EAD elements below are not mapped to the terms above: 

<ead> – EAD wrapper
<eadheader> – EAD Header
<filedesc> –  File Description 

-->

<!---

List of EAD3 Elements: 

abbr
abstract
accessrestrict
accruals
acqinfo
address
addressline
agencycode
agencyname
agent
agenttype
altformavail
appraisal
archdesc
archref
arrangement
author
bibliography
bibref
bioghist
blockquote
c
c01
c02
c03
c04
c05
c06
c07
c08
c09
c10
c11
c12
chronitem
chronitemset
chronlist
citation
colspec
container
control
controlaccess
controlnote
conventiondeclaration
corpname
custodhist
dao
daoset
date
daterange
dateset
datesingle
defitem
descriptivenote
did
didnote
dimensions
dsc
ead
edition
editionstmt
emph
entry
event
eventdatetime
eventdescription
eventtype
expan
famname
filedesc
fileplan
footnote
foreign
fromdate
function
genreform
geogname
geographiccoordinates
head
head01
head02
head03
index
indexentry
item
label
langmaterial
language
languagedeclaration
languageset
lb
legalstatus
list
listhead
localcontrol
localtypedeclaration
maintenanceagency
maintenanceevent
maintenancehistory
maintenancestatus
materialspec
name
namegrp
notestmt
num
occupation
odd
originalsloc
origination
otheragencycode
otherfindaid
otherrecordid
p
part
persname
physdesc
physdescset
physdescstructured
physfacet
physloc
phystech
prefercite
processinfo
ptr
ptrgrp
publicationstatus
publicationstmt
publisher
quantity
quote
recordid
ref
relatedmaterial
relation
relationentry
relations
repository
representation
row
scopecontent
script
separatedmaterial
seriesstmt
source
sourceentry
sources
sponsor
subject
subtitle
table
tbody
term
tgroup
thead
title
titleproper
titlestmt
todate
unitdate
unitdatestructured
unitid
unittitle
unittype
userestrict

-->
