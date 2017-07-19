
Map editing context for the currently open map editor in SLADE.

## Properties

| Property | Type | Description |
|:---------|:-----|:------------|
<prop>editMode</prop>        | <type>[mapEditor.Mode](../Namespaces/MapEditor.md#mode)</type> | The current edit mode
<prop>sectorEditMode</prop>  | <type>[mapEditor.SectorMode](../Namespaces/MapEditor.md#sectormode)</type> | The current sector edit mode
<prop>gridSize</prop>        | <type>number</type> | The current grid size
<prop>map</prop>             | <type>[Map](Map.md)</type> | The map associated with this editor

## Constructors

!!! attention "No Constructors"
    This type can not be created directly in scripts.

## Functions

### `selectedVertices`

<params>Parameters</params>

* `[`<type>boolean</type> <arg>tryHighlight</arg> : `false]`: Whether to get the current highlight if nothing is selected

**Returns** <type>[MapVertex](MapVertex.md)\[\]</type>

Returns an array of all currently selected vertices. If nothing is selected and <arg>tryHighlight</arg> is `true`, the currently highlighted vertex is returned in the array.

---
### `selectedLines`

<params>Parameters</params>

* `[`<type>boolean</type> <arg>tryHighlight</arg> : `false]`: Whether to get the current highlight if nothing is selected

**Returns** <type>[MapLine](MapLine.md)\[\]</type>

Returns an array of all currently selected lines. If nothing is selected and <arg>tryHighlight</arg> is `true`, the currently highlighted line is returned in the array.

---
### `selectedSectors`

<params>Parameters</params>

* `[`<type>boolean</type> <arg>tryHighlight</arg> : `false]`: Whether to get the current highlight if nothing is selected

**Returns** <type>[MapSector](MapSector.md)\[\]</type>

Returns an array of all currently selected sectors. If nothing is selected and <arg>tryHighlight</arg> is `true`, the currently highlighted sector is returned in the array.

---
### `selectedThings`

<params>Parameters</params>

* `[`<type>boolean</type> <arg>tryHighlight</arg> : `false]`: Whether to get the current highlight if nothing is selected

**Returns** <type>[MapThing](MapThing.md)\[\]</type>

Returns an array of all currently selected things. If nothing is selected and <arg>tryHighlight</arg> is `true`, the currently highlighted thing is returned in the array.

---
### `clearSelection`

Deselects all currently selected items

---
### `select`

<params>Parameters</params>

* <type>[MapObject](MapObject.md)</type> <arg>object</arg>: The <type>[MapObject](MapObject.md)</type> to (de)select
* `[`<type>boolean</type> <arg>select</arg> : `true]`: Whether to select or deselect the object

Selects or deselects the given <type>[MapObject](MapObject.md)</type> (or derived type), depending on <arg>select</arg>.