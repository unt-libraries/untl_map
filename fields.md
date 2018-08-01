##Overview
This list provides general information for each field element used in UNTL (University of North Texas Libraries) metadata records.  

Each table includes the following information:

- Description -- Definition of the field element.
- Required -- Whether or not a value is required for every record in the Digital Collections (Yes/No).
- Repeatable -- Whether or not the field is a repeatable element (Yes/No).
- Qualifier -- Link to the controlled vocabulary values for the field's qualifier, when applicable.
- Value Type -- Type of text value entered into the field, with links to vocabularies if the field value is strictly controlled.
- Guidelines -- Link to full explanation of field usage, input rules, and example values.
- Notes -- Other relevant notes, links, and applicable authorities or vocabularies that apply to the field.



##List of Fields

||**Title**|
|-------------------------------|------------------------------------------|
|Description | The name given to the resource.|
|Required | Yes|
|Repeatable | Yes|
|Qualifier | http://purl.org/NET/UNTL/vocabularies/title-qualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/title|
|Notes | Main title is required.|


||**Creator**|
|-------------------------------|------------------------------------------|
|Description | A person, agency, or organization primarily responsible for creating the intellectual content of the resource.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://purl.org/NET/UNTL/vocabularies/agent-qualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/creator|
|Notes | Every creator entry must include a role (qualifier) and type, with an optional information statement. Creator type value: http://digital2.library.unt.edu/vocabularies/agent-type/  <br /><br />Except for specific collections, an agent may only be listed once per record as a creator or contributor, but may be listed once as creator/contributor and also as publisher.<br /><br /> When possible, names should come from an established authority, including Library of Congress, the Virtual International Authority File (VIAF), or the local UNT Name App: http://digital2.library.unt.edu/name/|


||**Contributor**|
|-------------------------------|------------------------------------------|
|Description | A person or organization that has played an important but secondary role in creating the content of the resource and is not specified in the creator element.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://purl.org/NET/UNTL/vocabularies/agent-qualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/contributor|
|Notes | Every contributor entry must include a role (qualifier) and type, with an optional information statement.  Contributor type value: http://digital2.library.unt.edu/vocabularies/agent-type/  <br /><br /> Except for specific collections, an agent may only be listed once per record as a creator or contributor, but may be listed once as creator/contributor and also as publisher. <br /><br /> When possible, names should come from an established authority, including Library of Congress, the Virtual International Authority File (VIAF), or the local UNT Name App: http://digital2.library.unt.edu/name/|


||**Publisher**|
|-------------------------------|------------------------------------------|
|Description | An entity responsible for making the resource available: the publisher of the original work.|
|Required | No|
|Repeatable | Yes|
|Qualifier | No|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/publisher|
|Notes | Publisher should include a name and/or publication location, with optional information statement. <br /><br /> When possible, names should come from an established authority, including Library of Congress, the Virtual International Authority File (VIAF), or the local UNT Name App: http://digital2.library.unt.edu/name/|


||**Date**|
|-------------------------------|------------------------------------------|
|Description | Dates associated with events in the life cycle of the resource.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/date-qualifiers/|
|Value Type | EDTF Date|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/date|
|Notes | Date values must comply with the Extended Date/Time Format. <br /><br /> Each date type may only be used once per record.|


||**Language**|
|-------------------------------|------------------------------------------|
|Description | The language(s) of the intellectual content of the resource.|
|Required | Yes|
|Repeatable | Yes|
|Qualifier | No|
|Value Type | http://digital2.library.unt.edu/vocabularies/languages/|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/language|
|Notes | Language codes align with the ISO 639-2 specification.|


||**Description**|
|-------------------------------|------------------------------------------|
|Description | Description of the content and physical attributes of the resource.|
|Required | Yes|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/description-qualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/description|
|Notes | Content description is required. <br /><br /> Each description type may only be used once per record.|


||**Subject**|
|-------------------------------|------------------------------------------|
|Description | The subjects or topics that succinctly describe the content of the resource.|
|Required | Yes|
|Repeatable | Yes|
|Qualifier | http://purl.org/NET/UNTL/vocabularies/subject-qualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/subject|
|Notes | Two subjects of any type are required. <br /><br /> For all Portal records at least one value from the UNTL-BS is required: http://digital2.library.unt.edu/subjects/ <br /><br /> Subjects from controlled vocabularies must be authorized terms.|


||**Primary Source**|
|-------------------------------|------------------------------------------|
|Description | The primary source field designates firsthand accounts of historical subjects.|
|Required | No|
|Repeatable | No|
|Qualifier | No|
|Value Type | "0 = Not a primary source|
|1 = Item is a primary source"|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/primary-source|
|Notes | This is a local field.|


||**Coverage**|
|-------------------------------|------------------------------------------|
|Description | Geographic and temporal information related to the content of the resource.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://purl.org/NET/UNTL/vocabularies/coverage-eras/|
|Value Type | "Place Box: Geocode (http://www.dublincore.org/documents/dcmi-box/)|
|Place Name: Text string|
|Place Point: Geocode (http://dublincore.org/documents/dcmi-point/)|
|Coverage Date: EDTF Date|
|Time Period: http://purl.org/NET/UNTL/vocabularies/coverage-eras/"|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/coverage|
|Notes | Date entries cannot be repeated. <br /><br /> Date values must comply with the Extended Date/Time Format.|


||**Source**|
|-------------------------------|------------------------------------------|
|Description | Information about a resource from which the current resource is derived.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/sourceQualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/source|
|Notes | |


||**Citation**|
|-------------------------------|------------------------------------------|
|Description | Information about a serial item, a resource from which the current resource is derived, or peer-reviewed status of items.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/citationQualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/citation|
|Notes | This is a local field. <br /><br /> Each citation type may only be used once per record. <br /><br /> Value for “Peer Reviewed” is True/False; all others are text.|


||**Relation**|
|-------------------------------|------------------------------------------|
|Description | Information about another resource that is related to the current resource.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/relation-qualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/relation|
|Notes | |


||**Collection**|
|-------------------------------|------------------------------------------|
|Description | Collection refers to a larger group of resources with a unique collective title to which the resource being described belongs.|
|Required | Yes|
|Repeatable | Yes|
|Qualifier | No|
|Value Type | http://digital2.library.unt.edu/vocabularies/collections/|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/collection|
|Notes | This is a local field.|


||**Institution**|
|-------------------------------|------------------------------------------|
|Description | A consistent reference to the institution or administrative unit that owns the original resource for which metadata was created, or that retains rights and responsibilities related to the item and its usage.|
|Required | Yes|
|Repeatable | No|
|Qualifier | No|
|Value Type | http://digital2.library.unt.edu/vocabularies/institutions/|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/institution|
|Notes | This is a local field. <br /><br /> Same as “Partner” in public interfaces.|


||**Rights**|
|-------------------------------|------------------------------------------|
|Description | Rights information provides information about rights held in and over the resource; describes the conditions under which the work may be used, distributed, reproduced, etc.; how these conditions may change over time; and whom to contact regarding the copyright of the work.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/rights-qualifiers/|
|Value Type | "Access: http://digital2.library.unt.edu/vocabularies/rights-access/|
|Holder: Text string|
|License: http://digital2.library.unt.edu/vocabularies/rights-licenses/|
|Statement: Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/rights|
|Notes | |


||**Resource Type**|
|-------------------------------|------------------------------------------|
|Description | The type or category of the primary content of the resource.|
|Required | Yes|
|Repeatable | No|
|Qualifier | No|
|Value Type | http://digital2.library.unt.edu/vocabularies/resource-types/|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/resource-type|
|Notes | |


||**Format**|
|-------------------------------|------------------------------------------|
|Description | The digital manifestation of the resource.|
|Required | Yes|
|Repeatable | No|
|Qualifier | No|
|Value Type | http://digital2.library.unt.edu/vocabularies/formats/|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/format|
|Notes | |


||**Identifier**|
|-------------------------------|------------------------------------------|
|Description | A numeric or alphanumeric string or a URL that identifies the item in a particular context.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/identifier-qualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/identifier|
|Notes | Every item in the Digital Collections is assigned a unique, permanent ARK identifier during upload; that value is saved in the record’s administrative metadata.|


||**Degree**|
|-------------------------------|------------------------------------------|
|Description | Information about an originating agency, used specifically for theses/dissertations and for items created at the University of North Texas.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/degree-information/|
|Value Type | "College: Text string|
|Department: Text string|
|Discipline: Text string|
|Grantor: Text string|
|Level: http://digital2.library.unt.edu/vocabularies/degree-levels/|
|Name: Text string|
|Publication Type: http://digital2.library.unt.edu/vocabularies/publication-types/"|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/degree-information|
|Notes | This is a local field. <br /><br /> Each degree information type may only be used once per record.|


||**Note**|
|-------------------------------|------------------------------------------|
|Description | A "catch-all" field for additional information that cannot be entered or does not fit well in other elements.|
|Required | No|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/note-qualifiers/|
|Value Type | Text string|
|Guidelines | http://www.library.unt.edu/digital-projects-unit/note|
|Notes | This is a local field.|


||**Meta**|
|-------------------------------|------------------------------------------|
|Description | Information captured by the digital library system.|
|Required | Yes|
|Repeatable | Yes|
|Qualifier | http://digital2.library.unt.edu/vocabularies/meta-qualifiers/|
|Value Type | |
|Guidelines | http://www.library.unt.edu/digital-projects-unit/meta-information|
|Notes | This is a local field. <br /><br /> This field is automatically generated and updated by the system to document administrative information about the item and record, including permanent identifiers, dates of creation/edits, editors, etc. <br /><br /> Only specific components of the information can be edited (e.g., record status and system), and only by designated administrators.|
