# Constraints

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema.

**Prerequisites**

**Test method**

The following check is performed for every feature in the dataset.

* Check that values of [lowerBound](#lowerBound) element of the VerticalExtentRangeType data type are expressed in meters (OCL: "inv: self.lowerbound.uom.uomSymbol='m'").

* Check that values of [upperBound](#upperBound) element of the VerticalExtentRangeType data type are expressed in meters (OCL: "inv: self.upperBound.uom.uomSymbol='m'").

* Check that values of [scalar](#scalar) element of the VerticalExtentValue union type are expressed in meters (OCL: "inv: self.scalar.uom.uomSymbol='m'").


**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS-ER](./README.md#ref_TG_DS_ER) 5.4.2.1.1.

**Test type**: Automated

**Notes** 

Verify that the OCL constraints that are specified in the UML model of the application schema are met, i.e. validate features against the constraints. For unmet constraints report [constraintViolation](#constraintViolation).

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
constraintViolation <a name="constraintViolation"/>  |  XML document '$filename', $featureType '$gmlid': The constraint '$constraint' is violated.

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                   |  XPath expression                 |Multiplicity       |Voidable
------------------------------ | --------------------------------- | ------------------|----------
lowerBound <a name="lowerBound"></a> | //schema-element(er-v:FossilFuelResource)/er-v:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:range/er-b:VerticalExtentRangeType/er-b:lowerBound/@uom="m" <br> //schema-element(er-v:RenewableAndWasteResource)/er-v:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:range/er-b:VerticalExtentRangeType/er-b:lowerBound/@uom="m" <br> //schema-element(er-c:RenewableAndWastePotentialCoverage)/er-c:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:range/er-b:VerticalExtentRangeType/er-b:lowerBound/@uom="m" | Not applicable | Not applicable
upperBound <a name="upperBound"></a> | //schema-element(er-v:FossilFuelResource)/er-v:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:range/er-b:VerticalExtentRangeType/er-b:upperBound/@uom="m" <br> //schema-element(er-v:RenewableAndWasteResource)/er-v:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:range/er-b:VerticalExtentRangeType/er-b:upperBound/@uom="m" <br> //schema-element(er-c:RenewableAndWastePotentialCoverage)/er-c:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:range/er-b:VerticalExtentRangeType/er-b:upperBound/@uom="m" | Not applicable | Not applicable
scalar <a name="scalar"></a> | //schema-element(er-v:FossilFuelResource)/er-v:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:scalar/@uom="m" <br> //schema-element(er-v:RenewableAndWasteResource)/er-v:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:scalar/@uom="m" <br> //schema-element(er-c:RenewableAndWastePotentialCoverage)/er-c:verticalExtent/er-b:VerticalExtentType/er-b:verticalExtent/er-b:VerticalExtentValue/er-b:scalar/@uom="m" | Not applicable | Not applicable