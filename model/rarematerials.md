<!---

This document is a draft of work being done by the Task Force to Explore Data Elements for Rare Materials Description. 

Proposal
A Bibliographic Standards Committee (BSC) task force is proposed to explore and document data elements needed for rare materials description.  The task force will convene for one year, concluding its work prior to, and reporting at, the BSC meeting held at the 2016 ALA Annual Conference & Exhibition.
 
Charge
To determine a list of data elements complementary to the Descriptive Cataloging of Rare Materials (DCRM) suite, the RBMS Policy Statements for RDA, the Controlled Vocabularies for Use in Rare Book and Special Collections Cataloging, and rare materials user needs
To recommend solution(s) for incorporating these data elements into library and archives data models, schemata, and tools
To seek community partners for these solution(s)
 
Volunteers
· Allison Jai O’Dell, Metadata Librarian, University of Florida Libraries (task force chair, BSC member)
· Amy Tims, Project Cataloger, American Antiquarian Society (BSC member)
· Arielle Middleman, Cataloger, Library Company of Philadelphia (volunteer)
· Dot Porter, Curator of Digital Research Services, Kislak Center for Special Collections, Rare Books and Manuscripts, Penn Libraries (volunteer)
· Linde M. Brocato, Catalog Librarian, University of Memphis (volunteer)
· Amber D’Ambrosio, Special Collections Librarian and Archivist, Dixie State University Library (volunteer)
· Maria Oldal, Head of Cataloging and Database Maintenance, The Morgan Library and Museum (volunteer)
· Gloria Gonzalez, Library Strategist, Zepheira (volunteer)

For more information visit: http://derm.pbworks.com/w/page/99120051/FrontPage

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
    * @base: http://bibfra.me/vocab/rarematerials/
    * @property: http://bibfra.me/purl/versa/support
* title: Rare Materials Data Elements
* @interpretations:
    * scope: @resource


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
