<!---

RARE MATERIALS RELATION is a starting point for scoping data elements from RBMS Relationship Designators. It is inteneded to demonstrate how http://www.rbms.info/vocabularies/relators can be defined as Linked Data. 

Terms below are mapped from http://www.rbms.info/vocabularies/relators. Terms from https://github.com/zepheira/bibframe/blob/master/model/bfrel.md are reused and expanded upon as needed. http://bibfra.me/vocab/relation is mostly extracted from MARC relator terms. For now, MARC relator abbreviations are kept as synonyms. 

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
* description: Entity responsible for creating a work by conceiving, and implementing, an original graphic design, drawing, painting, or other work of art
* remark: Use specific terms when possible (for example, for book illustrators, use illustrator)

## assignee
* label: assignee
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: asg
* description: Entity to whom a license for printing or publishing has been transferred

## associatedname
* label: associated name
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: asn
* description: Name associated with or found in an item or collection, but which cannot be determined to be that of a “former owner” or other relator indicative of provenance

## attributedname
* label: attributed name
* refines: <http://bibfra.me/vocab/lite/contributor>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: att
* description: Author, artist, etc. related to a work for which there is or once was substantial authority for designating that person as author, creator, etc.
* remark: Use for supposed name

## illustrator
* label: illustrator
* refines: <http://bibfra.me/vocab/relation/artist>
* scope: <http://bibfra.me/vocab/relation>
* synonyms: ill
* description: Person, family, or organization contributing to a resource by supplementing the primary content with drawings, diagrams, photographs, etc. If the work is primarily the artistic content created by this entity, use artist or photographer
