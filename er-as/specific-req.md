# Energy Resources theme-specific requirement

**Purpose**: Verify that, where the geometry of the spatial object is derived from another spatial object, the geometries of the two objects are consistent.

**Prerequisites**

**Test method**

Check manually that if the geometry of the spatial object is derived from another spatial object, the geometries of the two objects are consistent.


**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 12 (1)
* [TG DS-ER](./README.md#ref_TG_DS_ER) 5.5.1.3.

**Test type**: Manual

**Notes** 

In a few cases Energy Resources features derive their geometry from another existing spatial object, when the boundaries of the natural resource are unknown or undefined. A typical example is a mining area or permission zone that might represent an Energy Resource at the same time. In this rare case the geometries of both spatial objects shall be consistent.

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                   |  XPath expression                 |Multiplicity       |Voidable
------------------------------ | --------------------------------- | ------------------|----------
