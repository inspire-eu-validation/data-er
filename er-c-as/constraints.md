# Constraints

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema.

**Prerequisites**

**Test method**

The following check is performed for every feature in the dataset.

* **rangeSetValuesAreOfTypeMeasure**: Check manually that the values in the [range set](#rangeSet) are of type Measure. (OCL: inv: rangeSet.forAll(oclIsKindOf(Measure))).


**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS-ER](./README.md#ref_TG_DS_ER) 5.6.2.1.1.

**Test type**: Manual

**Notes** 

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression                     |Multiplicity       |Voidable
---------------------------------------------------------- | ------------------------------------- | ------------------|----------
rangeSet <a name="rangeSet"></a> | //schema-element(er-c:RenewableAndWastePotentialCoverage)/gml:rangeSet | 0..\* | No
