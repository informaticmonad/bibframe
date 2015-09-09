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
    * @base: http://bibfra.me/vocab/rare/
    * @property: http://bibfra.me/purl/versa/support
* title: Rare Materials Data Elements
* @interpretations:
    * scope: @resource

<!---

The terms below this comment are examples that can be copy & pasted as templates for new terms. To define a class use one hash # and to define a property use two ##. For example: 

```
# Resource

* synonyms: http://bibframe.org/vocab/Resource http://schema.org/Thing
* label: Resource
* description: Conceptual Resource
* properties: label description image link
```

A section defining a resource type (analogous to an RDF class), as indicated by convention in this case by a top-level header marker (`#`). The List (multiple lines starting with (`*` then space) defines properties of the resource, or really metaproperties in this case.

```
## property

* description: a relationship between two resources or a resource and literal data
* label: property
```

A section defining a property (analogous to an RDF property), as indicated by convention in this case by a second-level header marker (`##`). Again the List defines metaproperties of the property.

-->

## titleProper

* label: title proper
* refines: <http://bibfra.me/vocab/lite/title>
* synonyms: 
* description: The title proper
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: Required element.

## datePublication

* label: date publication
* refines: <http://bibfra.me/vocab/lite/providerDate>
* description: The date of publication.
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: Required element. Recommended ISO 8601 date.

## signature

* label: signature note
* refines: <http://bibfra.me/vocab/lite/note>
* description: Superscript numbers represent the number of leaves per gathering. A signature is letter, numeral, symbol, or a group of such characters, printed at the foot of the rectos of the first few leaves of an intended gathering for the purpose of aiding binders in correctly assembling the sections.
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

<!---

FYI - Task Force members can separate individual sections of the document using comments. 

-->

<!---
Below are binding terms edited by Arielle Middlemman. These are limited to terms from RBMS Controlled Vocabularies as of 9/9/2015

-->

