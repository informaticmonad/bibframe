<!---

RARE MATERIALS RELATION is a starting point for scoping data elements from RBMS Relationship Designators. It is inteneded to demonstrate how http://www.rbms.info/vocabularies/relators/alphabetical_list.htm can be defined as Linked Data. 

Terms below are mapped from http://www.rbms.info/vocabularies/relators/alphabetical_list. Terms from https://github.com/zepheira/bibframe/blob/master/model/bfrel.md are reused and expanded upon as needed. http://bibfra.me/vocab/relation is mostly extracted from MARC relator terms. For now, MARC relator abbreviations are kept as synonyms. 

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
    * @base: http://bibfra.me/vocab/relation/
    * @property: http://bibfra.me/purl/versa/support
* title: BIBFRAME RELATION vocabulary
* @interpretations:
    * scope: @resource

## annotator
* label: annotator
* refines: * refines: <http://bibfra.me/vocab/relation/associatedname>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: ann
* description: Writer of manuscript annotations on a printed item

## artist
* label: artist
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: art
* description: Agent responsible for creating a work by conceiving, and implementing, an original graphic design, drawing, painting, or other work of art
* remark: Use specific terms when possible (for example, for book illustrators, use illustrator)

## assignee
* label: assignee
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: asg
* description: Agent to whom a license for printing or publishing has been transferred

## associatedName
* label: associated name
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: asn
* description: Name associated with or found in an item or collection, but which cannot be determined to be that of a “former owner” or other relator indicative of provenance

## attributedName
* label: attributed name
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: att
* description: Author, artist, etc. related to a work for which there is or once was substantial authority for designating that person as author, creator, etc.
* remark: Use for supposed name

## binder
* label: binder
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: bnd
* description: A person who binds an item

## bindingDesigner
* label: binding designer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: bdd
* description: A person or organization responsible for the binding design of a book, including the type of binding, the type of materials used, and any decorative aspects of the binding

## blurbWriter
* label: blurb writer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: blw
* description: Agent responsible for writing a commendation or testimonial for a work, which appears on or within the publication itself, frequently on the back or dust jacket of print publications or on advertising material for all media

## bookArtist
* label: book artist
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: bsl
* description: Agent who conceives and perhaps also executes an artist's book

## bookDesigner
* label: book designer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: bkd
* description: Agent responsible for the entire graphic design of a book, including arrangement of type and illustration, choice of materials, and process used

## bookjacketDesigner
* label: bookjacket designer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: bjd
* description: Agent responsible for the design of a dust jacket.

## bookplateDesigner
* label: bookplate designer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: bpd
* description: Agent responsible for the design of a book owner's identification label that is most commonly pasted to the inside front cover of a book

## bookseller
* label: bookseller
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: bsl
* description: Agent who makes books and other bibliographic materials available for purchase

## calligrapher
* label: calligrapher
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: cll
* description: Agent who writes in an artistic hand, usually as a copyist and or engrosser

## cartographer
* label: cartographer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: ctg
* description: Agent responsible for creating a map, atlas, globe, or other cartographic work

## censor
* label: censor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: cns
* description: Agent who examines bibliographic resources for the purpose of suppressing parts deemed objectionable on moral, political, military, or other grounds

## collector
* label: collector
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: col
* description: Agent responsible for bringing together material from various sources, which has been arranged, described, and cataloged as a collection

## collotyper
* label: collotyper
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: clt
* description: Agent involved in manufacturing a manifestation of photographic prints from film or other colloid that has ink-receptive and ink-repellent surfaces

## colorist
* label: colorist
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: clr
* description: Agent responsible for applying color to drawings, prints, photographs, maps, etc.

## compiler
* label: compiler
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: com
* description: Agent responsible for creating a new work (e.g., a bibliography, a directory) through the act of compilation, e.g., selecting, arranging, aggregating, and editing data, information, etc.

## compositor
* label: compositor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: cmt
* description: Agent responsible for the creation of metal slug, or molds made of other materials, used to produce the text and images in printed matter

## copyrightHolder
* label: copyright holder
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: cph
* description: Agent who created the intellectual content of a work or to whom copy and legal rights have been granted or transferred

## corrector
* label: corrector
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: crr
* description: Agent who is a corrector of manuscripts, such as the scriptorium official who corrected the work of a scribe

## correspondent
* label: correspondent
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: crp
* description: Agent who was either the writer or recipient of a letter or other communication

## contributor
* label: contributor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: ctb
* description: A person, family or organization responsible for making contributions to the resource. This includes those whose work has been contributed to a larger work, such as an anthology, serial publication, or other compilation of individual works. If a more specific role is available, prefer that, e.g. editor, compiler, illustrator.

## coverdesigner
* label: cover designer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: cov
* description: A person or organization responsible for the graphic design of a book cover, album cover, slipcase, box, container, etc. For a person or organization responsible for the graphic design of an entire book, use Book designer; for book jackets, use Bookjacket designer

## dedicatee
* label: dedicatee
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: dte
* description: Agent to whom a resource is dedicated

## dedicator
* label: dedicator
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: dto
* description: Agent who writes a dedication

## depositor
* label: depositor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: dpt
* description: Current owner of an item who deposited the item into the custody of another agent while still retaining ownership

## distributor
* label: distributor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: dst
* description: Agent that has exclusive or shared marketing rights for a resource

## donor
* label: donor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: dnr
* description: Former owner of an item who donated that item to another owner

## draftsman
* label: draftsman
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: drm
* description: Agent contributing to a resource by an architect, inventor, etc., by making detailed plans or drawings for buildings, ships, aircraft, machines, objects, etc.





## illustrator
* label: illustrator
* refines: <http://bibfra.me/vocab/relation/artist>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: ill
* description: Person, family, or organization contributing to a resource by supplementing the primary content with drawings, diagrams, photographs, etc. If the work is primarily the artistic content created by this entity, use artist or photographer
