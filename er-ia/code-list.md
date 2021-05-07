# Code lists

**Purpose**: Verify that code lists extensions can be accessed.

**Prerequisites**

**Test method**

* Verify that any code list extensions are publicly accessible via HTTP, i.e. inspect extensible code list values property elements. If a reference (@xlink:href) has a value that does not start with http://inspire.ec.europa.eu/codelist/, verify that a HTTP GET request to the URI retrieves a document. Otherwise report [brokenLink](#brokenLink).

This data theme currently has the following empty code lists:

* [ClassificationAndQuantificationFrameworkValue](#ClassificationAndQuantificationFrameworkValue): http://inspire.ec.europa.eu/codelist/ClassificationAndQuantificationFrameworkValue

* [FossilFuelClassValue](#FossilFuelClassValue): http://inspire.ec.europa.eu/codelist/FossilFuelClassValue

* [VerticalReferenceValue](#VerticalReferenceValue): http://inspire.ec.europa.eu/codelist/VerticalReferenceValue

* [PotentialTypeValue](#PotentialTypeValue): http://inspire.ec.europa.eu/codelist/PotentialTypeValue


**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (3)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP. Every code list value must be made available in an online registry. 

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression      |Multiplicity   |Voidable
---------------------------------------------------------- | -----------------------|---------------|---------------------------------
ClassificationAndQuantificationFrameworkValue <a name="ClassificationAndQuantificationFrameworkValue"></a> | //schema-element(er-v:FossilFuelResource)/er-v:ClassificationAndQuantificationFramework/@xlink:href <br> //schema-element(er-v:RenewableAndWasteResource)/er-v:ClassificationAndQuantificationFramework/@xlink:href | 0..1 | No
FossilFuelClassValue <a name="FossilFuelClassValue"></a> | //schema-element(er-v:FossilFuelResource)/er-v:resource/er-v:FossilFuelResourceType/er-v:quantity/er-v:FossilFuelMeasure/er-v:resourceClass/@xlink:href | 1 (0..\* for the parent) | No
VerticalReferenceValue <a name="VerticalReferenceValue"></a> | //schema-element(er-v:FossilFuelResource)/er-v:verticalExtent/er-b:VerticalExtentType/er-b:verticalReference/@xlink:href <br> //schema-element(er-v:RenewableAndWasteResource)/er-v:verticalExtent/er-b:VerticalExtentType/er-b:verticalReference/@xlink:href <br> //schema-element(er-c:RenewableAndWastePotentialCoverage)/er-c:verticalExtent/er-b:VerticalExtentType/er-b:verticalReference/@xlink:href | 1 | No
PotentialTypeValue <a name="PotentialTypeValue"></a> | //schema-element(er-c:RenewableAndWastePotentialCoverage)/er-c:potentialType/@xlink:href | 1 | No