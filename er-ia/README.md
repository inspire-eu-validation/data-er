# Conformance class: Information accessibility, Land Cover

Conformance class for the requirements related to the accessibility of referenced information, for example, information stored in registries (code lists, coordinate reference systems).

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Land Cover".

This conformance class is part of the [INSPIRE Data Specification on Land Cover](../README.md).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the data set, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](#ref_TG_DS_tmpl) | [Information accessibility](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-LC](#ref_TG_DS_LC) | [GML application schemas, Land Cover](../lc-gml/README.md) | INSPIRE spatial data set encoded in GML, Land Cover features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types are:

* For vector datasets:

	* FossilFuelResource
	* RenewableAndWasteResource

* For coverage datasets:

	* RenewableAndWastePotentialCoverage


*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-LC <a name="ref_TG_DS_LC"></a>   | [INSPIRE Data Specification on Land Cover – Technical Guidelines version 3.0](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_LC_v3.0.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-LC](#ref_TG_DS_LC)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code lists](./code-list.md)  | ready for review  | A.5.1 |


## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
gml            | http://www.opengis.net/gml/3.2
er-b    	       | http://inspire.ec.europa.eu/schemas/er-b/4.0
er-c		 	   | http://inspire.ec.europa.eu/schemas/er-c/4.0
er-v		 	   | http://inspire.ec.europa.eu/schemas/er-v/4.0

The following variables are used to refer to the corresponding Xpath expressions in all test descriptions:

Variable       | Value
-------------- | -------------------------------------------------
$features      |  //schema-element(er-v:FossilFuelResource) \| //schema-element(er-v:RenewableAndWasteResource) \| //schema-element(er-c:RenewableAndWastePotentialCoverage)