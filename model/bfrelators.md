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
* description: Person who binds an item

## bindingDesigner
* label: binding designer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: bdd
* description: Person or organization responsible for the binding design of a book, including the type of binding, the type of materials used, and any decorative aspects of the binding

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
* refines: <http://bibfra.me/vocab/relation/electrotyper>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: clt
* description: Agent involved in manufacturing a manifestation of photographic prints from film or other colloid that has ink-receptive and ink-repellent surfaces

## colorist
* label: colorist
* refines: <http://bibfra.me/vocab/relation/artist>
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
* description: Person, family or organization responsible for making contributions to the resource. This includes those whose work has been contributed to a larger work, such as an anthology, serial publication, or other compilation of individual works. If a more specific role is available, prefer that, e.g. editor, compiler, illustrator.

## coverDesigner
* label: cover designer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: cov
* description: Person or organization responsible for the graphic design of a book cover, album cover, slipcase, box, container, etc. For a person or organization responsible for the graphic design of an entire book, use Book designer; for book jackets, use Bookjacket designer

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

## editor
* label: editor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: edt
* description: Agent responsible for preparing for publication a work not primarily his/her/its own, such as by elucidating text, adding introductory or other critical matter, or technically directing an editorial staff

## electrotyper
* label: electrotyper
* refines: <http://bibfra.me/vocab/relation/platemaker>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: elt
* description: Agent who creates a duplicate printing surface by pressure molding and electrodepositing of metal that is then backed up with lead for printing

## engraver
* label: engraver
* refines: <http://bibfra.me/vocab/relation/artist>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: egr
* description: Agent who cuts letters, figures, etc. on a surface, such as a wooden or metal plate used for printing

## etcher
* label: etcher
* refines: <http://bibfra.me/vocab/relation/artist>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: etr
* description: Person or organization who produces text or images for printing by subjecting metal, glass, or some other surface to acid or the corrosive action of some other substance

## facsimilist
* label: facsimilist
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: etr
* description: Person or organization responsible for executing a facsimile or exact copy
* remark: Use for copier

## fore-edgePainter
* label: fore-edge painter
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: 
* description: Painter of a fore-edge painting
* remark: Use for fore-edge artist

## forger
* label: forger
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: 
* description: Agent who produces fraudulent copies or imitations
* remark: Use for copier and counterfeiter

## formerOwner
* label: former owner
* refines: <http://bibfra.me/vocab/relation/associatedName>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: fmo
* description: Agent who formerly had legal possession of an item
* remark: Use for inscribee

## graphictechnician
* label: graphic technician
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person responsible for preparing graphic drawings, maps, displays and other visual resources

## honoree
* label: honoree
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person, family, or organization honored by a work or item (e.g., the honoree of a festschrift, a person to whom a copy is presented)

## illustrator
* label: illustrator
* refines: <http://bibfra.me/vocab/relation/artist>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: ill
* description: Person, family, or organization contributing to a resource by supplementing the primary content with drawings, diagrams, photographs, etc. If the work is primarily the artistic content created by this entity, use artist or photographer

## illuminator
* label: illuminator
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person providing decoration to a specific item using precious metals or color, often with elaborate designs and motifs

## indexer
* label: indexer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Entity responsible for compiling an index. 

## inscriber
* label: inscriber
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person who has written a statement of dedication or gift. Use for the entity that signs a presentation statement.

## interviewee
* label: interviewee
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person, family or organization responsible for creating or contributing to a resource by responding to an interviewer, usually a reporter, pollster, or some other information gathering agent

## interviewer
* label: interviewer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person, family, or organization responsible for creating or contributing to a resource by acting as an interviewer, reporter, pollster, or some other information gathering agent

## lender
* label: lender
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization permitting the temporary use of a book, manuscript, etc., such as for photocopying or microfilming

## licensee
* label: licensee
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization who is an original recipient of the right to print or publish

## licensor
* label: licensor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization who is a signer of the license, imprimatur, etc.

## lithographer
* label: lithographer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization who prepares the stone or plate for lithographic printing, including a graphic artist creating a design directly on the surface from which printing will be done.

## marbler
* label: marbler
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: The entity responsible for marbling paper, cloth, leather, etc. used in construction of a resource

## medium
* label: medium
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person who purports to communicate with spirits.
* remark: Proposed by Laura O'Keefe, 8/03. Although modern specialist usage recognizes distinctions among the functions of "medium," "psychic," "channel," and "clairvoyant," these terms appear to be less distinct in earlier works. This accounts for the inclusion of UFs that are not strictly equivalent according to specialists in psychic phenomena.  

## metal-engraver
* label: metal-engraver
* refines: <http://bibfra.me/vocab/lite/engraver>
* scope: <http://bibfra.me/vocab/relation>
* description: Engraver responsible for decorations, illustrations, letters, etc. cut on a metal surface for printing or decoration

## paperEngineer
* label: paper engineer
* refines: <http://bibfra.me/vocab/lite/engraver>
* scope: <http://bibfra.me/vocab/relation>
* description: Person responsible for the design of mechanisms of three-dimensional paper structures found in movable and pop-up books, greeting cards, etc.

## papermaker
* label: papermaker
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization responsible for the production of paper, usually from wood, cloth, or other fibrous material

## patron
* label: patron
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization responsible for commissioning a work. For the entity assuming primary responsibility for the production of a work, that is, the entity under the auspices of which a work is printed, published, etc., use http://bibfra.me/vocab/relation/sponsor.

## photographer
* label: photographer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person, family, or organization responsible for creating a photographic work

## platemaker
* label: platemaker
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person, family, or organization involved in manufacturing a manifestation by preparing plates used in the production of printed images and/or text

## stereotyper
* label: stereotyper
* refines: <http://bibfra.me/vocab/lite/platemaker>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization who creates a new plate for printing by molding or copying another printing surface


## printerOfPlates
* label: printer of plates
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization who prints illustrations from plates.

## printmaker
* label: printmaker
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization who makes a relief, intaglio, or planographic printing surface

## proofreader
* label: proofreader
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person who corrects printed matter. For manuscripts, use Corrector [crr]

## publisher
* label: publisher
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization responsible for publishing, releasing, or issuing a resource

## recipient
* label: recipient
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Entity to whom correspondence is addressed.

## rubricator
* label: rubricator
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: A person or organization responsible for parts of a work, often headings or opening parts of a manuscript, that appear in a distinctive color, usually red

## scribe
* label: scribe
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: A person who is an amanuensis and for a writer of manuscripts proper. 
* remark: For a person who makes pen-facsimiles, use Facsimilist [fac]

## signer
* label: signer
* refines: <http://bibfra.me/vocab/lite/associatedname>
* scope: <http://bibfra.me/vocab/relation>
* description: A person whose signature appears without a presentation or other statement indicative of provenance. When there is a presentation statement, use Inscriber [ins].

## sponsor
* label: sponsor
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: A person, family, or organization sponsoring some aspect of a resource, e.g., funding research, sponsoring an event
* remark: For the entity responsible for commissioning a work, use Patron.

## stereotyper
* label: stereotyper
* refines: <http://bibfra.me/vocab/lite/platemaker>
* scope: <http://bibfra.me/vocab/relation>
* description: A person or organization who creates a new plate for printing by molding or copying another printing surface

## subscriber
* label: subscriber
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Entity responsible for purchasing or pledging to purchase an item in advance of its publication.
* remark: Use for a person who purchases or pledges to purchase an item in advance of its publication.  

## transcriber
* label: transcriber
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: A person, family, or organization contributing to a resource by changing it from one system of notation to another. For a work transcribed for a different instrument or performing group, see Arranger [arr]. For makers of pen-facsimiles, use Facsimilist [fac]

## typedesigner
* label: type designer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: A person or organization who designs the type face used in a particular item

## typographer
* label: typographer
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: A person or organization primarily responsible for choice and arrangement of type used in an item. If the typographer is also responsible for other aspects of the graphic design of a book (e.g., Book designer [bkd]), codes for both functions may be needed

## witness
* label: witness
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person who verifies the truthfulness of an event or action

## woodengraver
* label: wood engraver
* refines: <http://bibfra.me/vocab/lite/engraver>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization who makes prints by cutting the image in relief on the end-grain of a wood block

## woodcutter
* label: woodcutter
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person or organization who makes prints by cutting the image in relief on the plank side of a wood block
* 
## zinester
* label: zinester
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* description: Person who creates a zine








<!---

Approved: Scope notes for the following 12 terms have been finalized and will be added to the Controlled Vocabularies genre list in the next update: http://rbms.info/vocabularies/genre/alphabetical_list.htm
Academic dissertations
Abridgments
Novenas
Annual reports
Anniversary sermons
Anatomical atlases
Anagrams
Anthologies
Anti-homosexual literature
Anti-communist literature
Anti-clerical literature
Anti-Catholic literature
 
Deleted:
Alphabets
Oriental tales

Under-going comment until Aug 28:
Account books
Acrostics
Adaptations
Addresses
Advertisements
Publishers’ advertisements
Administrative regulations

MARC relators not included in RBMS terms - 

* editorofcompilation
* editorofmovingimagework

Notes: 

* platemaker/electrotyper/collotyper refinement

-->




