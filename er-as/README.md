# Conformance class: Application schema, Energy Resources Base

Conformance class for the requirements associated with the application schema. 

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Energy Resources".

This conformance class is part of the [INSPIRE Data Specification on Energy Resources](../README.md).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

none

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-ER](./README.md#ref_TG_DS_ER) | [GML application schemas, Energy Resources](../er-gml/README.md) | INSPIRE spatial data set encoded in GML, Energy Resources features | n/a |
 
## Feature types <a name="feature-types"></a>

This application schema defines only a data type and a code list, used by feature types defined in the other two application schemas, Energy Resources Coverage and Energy Resources Vector.


*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers to instances of feature types of the two application schemas, Energy Resources Coverage and Energy Resources Vector.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-ER <a name="ref_TG_DS_ER"></a>   | [INSPIRE Data Specification on Energy Resources – Technical Guidelines version 3.0](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_ER_v3.0.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-ER](#ref_TG_DS_ER)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code list values](./code-list-values.md)  | ready for review  | A.1.3  |
| [Constraints](./constraints.md)  | ready for review  | A.1.6  |
| [Specific requirements](./specific-req.md)  | ready for review  | A.1.6  |


## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
er-b    	 	   | http://inspire.ec.europa.eu/schemas/er-b/4.0
base           | http://inspire.ec.europa.eu/schemas/base/3.3
gml            | http://www.opengis.net/gml/3.2
wfs            | http://www.opengis.net/wfs/2.0
xsi            | http://www.w3.org/2001/XMLSchema-instance
xlink          | http://www.w3.org/1999/xlink
xml            | http://www.w3.org/XML/1998/namespace