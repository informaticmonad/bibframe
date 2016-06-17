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


<!-- TITLE -->

## titleSource

* label: title source
* refines: <http://bibfra.me/vocab/lite/title>
* description: Source of the title, used when not explicitly given on the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: Includes devised title

## correctedTitle

* label: Corrected Title
* refines: <http://bibfra.me/vocab/lite/titleAlternative>
* description: Title corrected by cataloging agency
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## preferredCitation

* label: preferred citation
* refines: <http://bibfra.me/vocab/archive>
* description: Phrasing for preferred citation when referencing the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- LANGUAGE -->

## translationOf

* label: translation of
* refines: <http://bibfra.me/vocab/lite/language> 	
* description: Relationship to resource which the resource is a translation of
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## translatedAs

* label: translated as
* refines: <http://bibfra.me/vocab/lite/language>
* description: Relationship to resource which is a translation of the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>


<!-- CONSTRUCTION -->

## collation

* label: collation
* refines: <http://bibfra.me/vocab/lite/note>
* synonyms: <http://bibfra.me/vocab/dcrmb/signature>
* description: Collation or signature statement
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: Suggest replacing <http://bibfra.me/vocab/dcrmb/signature> with collation, to encompass manuscript materials

## layout

* label: layout
* refines: <http://bibfra.me/vocab/marc/otherPhysicalDetails/>
* description: Description of page or other layout
* value: Literal
* scope: <http://bibfra.me/vocab/rare>
* remark: For maps, examples include “both sides”,“back to back”, and/or note to describe any other unusual layout of the map(s), etc.


<!-- CONDITION -->

## condition

* label: condition
* refines: <http://bibfra.me/vocab/rare>
* synonyms: 
* description: Condition report, including conservation/preservation needs and defects of the copy
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- HISTORY OF USE -->

## originCulture

* label: culture
* refines: <http://bibfra.me/vocab/rare>
* description: Culture from which the creation of the work originated
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## userEngagement

* label: user engagement
* refines: <http://bibfra.me/vocab/lite/note>
* description: Evidence of user or reader engagement, such as marks, inscriptions, and annotations
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## addedMaterials

* label: added materials
* refines: <http://bibfra.me/vocab/rare/userEngagement>
* description: Description of materials added to the resource by a user, such as extra-illustrations and insertions
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## userEngagementTerm

* label: user engagement term
* refines: <http://bibfra.me/vocab/rare>
* description: Index terms for evidence of user or reader engagement, such as marks, inscriptions, annotations, and added materials
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## shelfmark

* label: shelfmark
* refines: <http://bibfra.me/vocab/rare>
* description: Current and former shelfmarks
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- BINDING -->

## binding

* label: binding
* refines: <http://bibfra.me/vocab/lite/note>
* description: Description of bookbinding
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## sewing

* label: sewing
* refines: <http://bibfra.me/vocab/rare/binding>
* description: Description of sewing structures used in bookbinding
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## bindingDesign

* label: binding design
* refines: <http://bibfra.me/vocab/rare/binding>
* description: Description of surface design used in bookbinding, particularly of stylistic features and cultural/geographic/temporal context
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## cover

* label: cover
* refines: <http://bibfra.me/vocab/rare/binding>
* description: Description of covering materials, wrappers, jackets, etc.
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## bindingTerm

* label: binding term
* refines: <http://bibfra.me/vocab/rare/binding>
* description: Index terms for binding
* value: URI
* scope: <http://bibfra.me/vocab/rare>

##bindingColor

* label: binding color
* refines: <http://bibfra.me/vocab/marc/color>
* description: Index colors of bookbinding coloring material
* value: URI
* scope: <http://bibfra.me/vocab/rare>


<!-- CONTENTS -->

## boundWith

* label: bound with
* refines: <http://bibfra.me/vocab/rare>
* description: URI for bound-with resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## unnamedContents

* label: unnamed contents
* refines: <http://bibfra.me/vocab/marc/contentsNote>
* description: List contents not named on the title page
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## advertisement

* label: advertisement
* refines: <http://bibfra.me/vocab/marc/contentsNote>
* description: Note about advertisements included in the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## errata

* label: errata
* refines: <http://bibfra.me/vocab/marc/contentsNote>
* description: Note about errata slips
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## expansionCorrection

* label: expansion
* refines: <http://bibfra.me/vocab/lite/extent>
* description: Note on expansions or corrections
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- GRAPHICS & ILLUSTRATIONS -->

## printmaking

* label: printmaking
* refines: <http://bibfra.me/vocab/marc/illustrations>
* description: Description of printmaking processes used to make the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## printmakingTerm

* label: printmaking term
* refines: <http://bibfra.me/vocab/rare/printmaking>
* description: Index printmaking processes used to make the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## decoration

* label: decoration
* refines: <http://bibfra.me/vocab/marc/illustrations>
* description: Decorative features, as in illumination, historiation, designs, and patterns
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## decorationTerm

* label: decoration term
* refines: <http://bibfra.me/vocab/rare/decoration>
* description: Index decorative features
* value: URI
* scope: <http://bibfra.me/vocab/rare>


<!-- EXHIBITS -->

## exhibit

* label: exhibit history
* refines: <http://bibfra.me/vocab/dcrmb>
* description: Note about exhibitions that have featured the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## exhibitCatalog

* label: exhibit catalog
* refines: <http://bibfra.me/vocab/dcrmb/citations>
* description: Relationship to an exhibition catalog that features the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## exhibitOf

* label: exhibit of
* refines: <http://bibfra.me/vocab/dcrmb/citations>
* description: Relationship to resources featured in an exhibition catalog
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: Use contents note for literal explanation of exhibited resources


<!-- BIBLIOGRAPHIES -->

## citedIn

* label: cited in
* refines: <http://bibfra.me/vocab/rare/citations>
* synonyms: <http://bibfra.me/vocab/marc/citationUri>
* description: Relationship to a resource that cites the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: Suggest revision of <http://bibfra.me/vocab/marc/citationUri> to reflect citedIn / citedBy reflexive relationship

## cites

* label: cites
* refines: <http://bibfra.me/vocab/rare/citations>
* description: Relationship to a resource cited in the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>


<!-- EDITION -->

## limitationStatement

* label: limitation statement
* refines: <http://bibfra.me/vocab/marc/edition>
* description: Statement regarding editioning and/or the limited number of copies in an edition
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## colophon

* label: colophon
* refines: <http://bibfra.me/vocab/marc/edition>
* description: Transcription of the colophon
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## version

* label: version
* refines: <http://bibfra.me/vocab/marc/edition>
* description: Statement about the version of the resource, as in manuscript tradition
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## issue

* label: issue
* refines: <http://bibfra.me/vocab/marc/edition>
* description: Details about the particular issue of the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## state

* label: state
* refines: <http://bibfra.me/vocab/marc/edition>
* description: Details about the particular state of the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- SUBJECTS & GENRES -->

## depicts

* label: depicts
* refines: <http://bibfra.me/vocab/lite/subject>
* description: Index term for something or someone featured and/or depicted in/on the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: The ‘of-ness’ of a work

## application

* label: application
* refines: <http://bibfra.me/vocab/lite/subject>
* description: Index disciplines, methods, etc. which would likely find applications for the resource 
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: The ‘useful-ness’ of a work

## workType

* label: work type
* refines: <http://bibfra.me/vocab/lite/genre>
* description: Index the kind of work or works being described
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## style

* label: style
* refines: <http://bibfra.me/vocab/lite/genre>
* description: Index artistic or cultural styles used in the work
* value: URI
* scope: <http://bibfra.me/vocab/rare>


<!-- MATERIALS & TECHNIQUES -->

## technique

* label: technique
* refines: <http://bibfra.me/vocab/rare>
* description: Index techniques used to make the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## material

* label: material
* refines: <http://bibfra.me/vocab/rare>
* description: Index materials used to make the resource, such as leather, cloth, vellum, or paper fibers
* value: URI
* scope: <http://bibfra.me/vocab/rare>
 
## paper

* label: paper
* refines: <http://bibfra.me/vocab/lite/note>
* description: Description of paper used to make the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- DATES -->

## fictitiousDate

* label: fictitious date
* refines: <http://bibfra.me/vocab/lite/date>
* description: Fictitious date associated with the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## incorrectDate

* label: incorrect date
* refines: <http://bibfra.me/vocab/lite/date>
* description: Incorrect date associated with the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## situationDate

* label: situation date
* refines: <http://bibfra.me/vocab/lite/date>
* description: date (or dates) of the information shown on the material
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- COPYRIGHT -->

## freedomUse

* label: freedom to use
* refines: <http://bibfra.me/vocab/lite/copyright>
* description: Freedoms to use and/or reproduce content, such as creative commons or copyleft licenses
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## restrictionUse

* label: restrictions on use
* refines: <http://bibfra.me/vocab/lite/copyright>
* description: Restrictions on use or reproduction of the resource and its content, such as intellectual property rights or embargos
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- REPRODUCTION -->

## reproduction

* label: reproduction
* refines: <http://bibfra.me/vocab/marc/reproductionNote>
* description: Relationship to a reproduction of the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>


<!-- LETTERFORMS -->

## type

* label: type
* refines: <http://bibfra.me/vocab/rare>
* description: Description of type used to make the resource
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## typeTerm

* label: type term
* refines: <http://bibfra.me/vocab/rare/type>
* description: Index typefaces and type features used to make the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## script

* label: script
* refines: <http://bibfra.me/vocab/rare>
* description: Description of script(s) used to make the resource, as in calligraphy or manuscript hands
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## scriptTerm

* label: script term
* refines: <http://bibfra.me/vocab/rare/script>
* description: Index letterforms used to make the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>


<!--  SERIALS -->

## issuedAlsoAs

* label: issued also as
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to resource issued parallel to resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## supplementTo

* label: supplement to
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* synonyms: 
* description: Relationship to resource which the resource supplements
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: Includes issued between issues of relationship

## supplementedBy

* label: supplemented by
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to resource which supplements the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>
* remark: Includes issued with and indexes

## reissueOf

* label: re-issue of
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to a resource which the resource is a re-issue of
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## reissuedAs

* label: re-issued as
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to resource which the resouce was re-issued as
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## continues

* label: continues
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to resource that the resource continues
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## continuedBy

* label: continued by
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to resource that continues the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## merger

* label: merger
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to resource that the resource is a merger/absorption from, to, or with
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## splitInto

* label: split into
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to resource which was split from the resource
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## separatedFrom

* label: separated from
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to resource which the resource was separated from
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## variantOf

* label: variant of
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Relationship to a resource which the resource is a variant of
* value: URI
* scope: <http://bibfra.me/vocab/rare>

## numbering

* label: numbering
* refines: <http://bibfra.me/vocab/marc/ContinuingResources>
* description: Note about numbering schemes and/or irregularities
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## beganWith

* label: began with
* refines: <http://bibfra.me/vocab/rare/numbering>
* description: Issue which publication began with
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## ceasedWith

* label: ceased with
* refines: <http://bibfra.me/vocab/rare/numbering>
* description: Issue which publication ceased with
* value: Literal
* scope: <http://bibfra.me/vocab/rare>


<!-- MAPS -->

## scale

* label: scale
* refines: <http://bibfra.me/vocab/marc/remainderOfScale>
* description: Contains additional information regarding scale conversion from bar scale, verbal scale or lack of scale on item
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## scaleTranscription

* label: scale transcription
* refines: <http://bibfra.me/vocab/marc/remainderOfScale>
* description: Provides transcription of any scale present but not transcribed in another element
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## verticalScale

* label: vertical scale
* refines: <http://bibfra.me/vocab/marc/representativeFractionOfScale>
* description: The vertical scale or exaggeration of a 3D model
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## coordinates

* label: coordinates
* refines: <http://bibfra.me/vocab/rare>
* description: Provides coordinates of cartographic material
* describes: <http://bibfra.me/vocab/marc/Map/>
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## coordinatesNote

* label: coordinates note
* refines: <http://bibfra.me/vocab/rare/coordinates>
* description: Additional information about coordinates, such as coordinates not extending to neat line or prime meridian other than Greenwich
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## equinoxEpoch

* label: equinox and epoch
* refines: <http://bibfra.me/vocab/rare/coordinates/coordinatesNote>
* description: Statement of equinox or epoch for celestial materials
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## declinationLimit

* label: declination limit
* refines: <http://bibfra.me/vocab/rare/coordinates>
* description: For charts centered on one of the two poles, give the declination limit
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## declinationZones

* label: declination zones
* refines: <http://bibfra.me/vocab/rare/coordinates>
* description: 
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## mapDissected

* label: dissected map
* refines: <http://bibfra.me/vocab/marc/otherPhysicalDetails/>
* description: Indication if cartographic material has been dissected
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## mapMounted

* label: mounted map
* refines: <http://bibfra.me/vocab/marc/otherPhysicalDetails>
* description: Indication if map has been mounted
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## coverage

* label: coverage
* refines: <http://bibfra.me/vocab/lite/note>
* description: Geographic coverage of the material, unless apparent from the rest of the description
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## magnitude

* label: magnitude
* refines: <http://bibfra.me/vocab/rare/coordinates/coordinatesNote>
* description: Magnitude of celestial charts
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## dedication

* label: dedication note
* refines: <http://bibfra.me/vocab/lite/note>
* description: Grammatically separable dedications appearing in the chief source of information that have been omitted from the transcription
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## inset

* label: inset
* refines: < http://bibfra.me/vocab/rare>
* description: information relating to insets, ancillary maps, supplementary maps, maps on the verso of a sheet, illustrations, etc.
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## appearsIn

* label: appears in
* refines: < http://bibfra.me/vocab/rare>
* description: Relationship to work in which an identical plate appears, but cannot definitely be determined to be removed from
* value: URI
* scope: <http://bibfra.me/vocab/rare>


<!-- ARCHIVES & COLLECTIONS -->

## accruals

* label: accruals
* refines: <http://bibfra.me/vocab/archive>
* description: Information regarding accruals or planned additions to a collection
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

## retentionSchedule

* label: retention schedule
* refines: <http://bibfra.me/vocab/archive>
* description: Information about retention schedules or planned destruction
* value: Literal
* scope: <http://bibfra.me/vocab/rare>

