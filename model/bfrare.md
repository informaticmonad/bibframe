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
Below is a compilation of Arielle's, Amy's, and Allison's notes, excluding elements already in the bibfra.me vocab (sometimes under a different label)

-->

## limitationStatement

* label: Limitation Statement
* refines: <http://bibfra.me/vocab/marc/edition>
* synonyms: 
* description: Statement regarding editioning and/or the limited number of copies in an edition
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## correctedTitle

* label: Corrected Title
* refines: <http://bibfra.me/vocab/lite/titleAlternative>
* synonyms: 
* description: Title corrected by cataloging agency
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## condition

* label: Condition
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Condition report, including conservation/preservation needs
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 

## userEngagement

* label: User Engagement
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Evidence of user or reader engagement, such as marks, inscriptions, and annotations
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## addedMaterials

* label: Added Materials
* refines: <http://bibfra.me/vocab/dcrmb/userEngagement>
* synonyms: 
* description: Description of materials added to the resource by a user, such as extra-illustrations and insertions.
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## userEngagementTerm

* label: User Engagement Term
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Index terms for evidence of user or reader engagement, such as marks, inscriptions, annotations, and added materials
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## binding

* label: 
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Description of bookbinding
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## sewing

* label: 
* refines: <http://bibfra.me/vocab/dcrmb/binding>
* synonyms: 
* description: Description of sewing structures used in bookbinding
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## bindingDesign

* label: Cover Material
* refines: <http://bibfra.me/vocab/dcrmb/binding>
* synonyms: 
* description: Description of surface design used in bookbinding, particularly of stylistic features and cultural/geographic/temporal context
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## bindingTerm

* label: Binding Term
* refines: <http://bibfra.me/vocab/dcrmb/binding>
* synonyms: 
* description: Index terms for binding
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


##bindingColor

* label: Binding Color
* refines: <http://bibfra.me/vocab/dcrmb/binding/bindingTerm>
* synonyms: 
* description: Index colors of bookbinding coloring material
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## boundWith

* label: Bound With
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: URI for bound-with resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## technique

* label: Technique
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Index techniques used to make the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## material

* label: Material
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Index materials used to make the resource, such as leather, cloth, vellum, or paper fibers
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 
 

## paper

* label: Paper
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Description of paper used to make the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## type

* label: Type
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Description of type used to make the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## typeTerm

* label: Type Term
* refines: <http://bibfra.me/vocab/dcrmb/type>
* synonyms: 
* description: Index typefaces and type features used to make the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## printmaking

* label: Printmaking
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Description of printmaking processes used to make the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## printmakingTerm

* label: Printmaking Term
* refines: <http://bibfra.me/vocab/dcrmb/printmaking>
* synonyms: 
* description: Index printmaking processes used to make the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark:  


## exhibition

* label: Exhibition History
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Note about exhibitions that have featured the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## exhibitionCatalog

* label: Featured in Exhibition Catalog
* refines: <http://bibfra.me/vocab/dcrmb/citations>
* synonyms: 
* description: Relationship to an exhibition catalog that features the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## exhibitionOf

* label: Exhibition of
* refines: <http://bibfra.me/vocab/dcrmb/citations>
* synonyms: 
* description: Relationship to resources featured in an exhibition catalog
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## citedIn

* label: Cited In
* refines: <http://bibfra.me/vocab/dcrmb/citations>
* synonyms: <http://bibfra.me/vocab/marc/citationUri>
* description: Relationship to a resource that cites the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: Suggest revision of <http://bibfra.me/vocab/marc/citationUri> to reflect citedIn / citedBy reflexive relationship


## cites

* label: Cites
* refines: <http://bibfra.me/vocab/dcrmb/citations>
* synonyms: 
* description: Relationship to a resource cited in the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## reproduction

* label: Reproduction
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Relationship to a reproduction of the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## preferredCitation

* label: Preferred Citation
* refines: <http://bibfra.me/vocab/>
* synonyms: 
* description: Phrasing for preferred citation when referencing the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## issue

* label: Issue
* refines: <http://bibfra.me/vocab/marc/edition>
* synonyms: 
* description: Details about the particular issue of the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## state

* label: State
* refines: <http://bibfra.me/vocab/marc/edition>
* synonyms: 
* description: Details about the particular state of the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## advertisement

* label: Advertisement for
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Note about advertisements included in the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## errata

* label: Errata
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Note about errata slips
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## originCulture

* label: Culture
* refines: <http://bibfra.me/vocab/marc>
* synonyms: 
* description: Culture from which the creation of the work originated
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## depicts

* label: Depicts
* refines: <http://bibfra.me/vocab/lite/subject>
* synonyms: 
* description: Index term for something or someone featured and/or depicted in/on the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: The ‘of-ness’ of a work


## researchApplication

* label: Research Application
* refines: <http://bibfra.me/vocab/lite/subject>
* synonyms: 
* description: Index disciplines, methods, etc. which would likely find applications for the resource 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: The ‘useful-ness’ of a work


## workType

* label: Work Type
* refines: <http://bibfra.me/vocab/lite/genre>
* synonyms: 
* description: Index the kind of work or works being described
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## style

* label: Style
* refines: <http://bibfra.me/vocab/lite/genre>
* synonyms: 
* description: Index artistic or cultural styles used in the work
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 




## fictitiousDate

* label: Fictitious Date
* refines: <http://bibfra.me/vocab/lite/date>
* synonyms: 
* description: Fictitious date associated with the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## incorrectDate

* label: Incorrect Date
* refines: <http://bibfra.me/vocab/lite/date>
* synonyms: 
* description: Incorrect date associated with the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## freedomUse

* label: Freedom to Use
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Freedoms to use content, such as creative commons licenses
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## restrictionUse

* label: Restrictions on Use
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Restrictions on access or use of the resource and its content, such as intellectual property rights or embargos
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## titleSource

* label: Title Source
* refines: <http://bibfra.me/vocab/lite/title>
* synonyms: 
* description: Source of the title, used when not explicitly given on the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: Includes devised title


## translationOf

* label: Translation of
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## translatedAs

* label: Translated as
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## issuedAlsoAs

* label: Issued Also as
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## supplementTo

* label: Supplement to
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## supplementedBy

* label: Supplemented by
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: Includes issued with and indexes



<!--  Serials-specific stuff below -->

## reissueOf

* label: Re-issue of
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Relationship to a resource which the resource is a re-issue of
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## reissuedAs

* label: Re-issued as
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## continues

* label: Continues
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## continuedBy

* label: Continued by
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## mergerOf

* label: Merger of
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: Includes merger of and absorbed


## mergedWith

* label: Merged with
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: Includes merged with and absorbed into


## splitInto

* label: Split into
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## separatedFrom

* label: Separated from
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 

## variantOf

* label: Variant of
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Relationship to a resource which the resource is a variant of
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## numbering

* label: Numbering
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Note about numbering schemes, especially used for series and serials
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## numbering

* label: Numbering
* refines: <http://bibfra.me/vocab/dcrmb>
* synonyms: 
* description: Note about numbering schemes, especially used for series and serials
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## beganWith

* label: Began with
* refines: <http://bibfra.me/vocab/dcrmb/numbering>
* synonyms: 
* description: 
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## ceasedWith

* label: Ceased with
* refines: <http://bibfra.me/vocab/dcrmb/numbering>
* synonyms: 
* description: 
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: 


## betweenIssuesOf

* label: Issued Between Issues of
* refines: <http://bibfra.me/vocab/lite/title>
* synonyms: 
* description: 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: 

