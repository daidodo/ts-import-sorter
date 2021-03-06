# Interface: Configuration

## Properties

### bracketSpacing

• `Optional` `Readonly` **bracketSpacing**: *boolean*

Whether to add spaces between brackets. _true_ for '{ id }' and _false_ for '{id}'. Default to
_true_.

Defined in: [config/types/index.ts:128](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L128)

___

### configurationFileName

• `Optional` `Readonly` **configurationFileName**: *string*

JSON configuration file name. Default to _import-sorter.json_.

Defined in: [config/types/index.ts:19](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L19)

___

### emptyLinesAfterAllImports

• `Optional` `Readonly` **emptyLinesAfterAllImports**: *number*

Number of empty lines after the last import declaration. Default to _1_.

Defined in: [config/types/index.ts:87](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L87)

___

### emptyLinesBetweenGroups

• `Optional` `Readonly` **emptyLinesBetweenGroups**: *number*

Number of empty lines between groups (NOT sub-groups). Default to _1_.

Defined in: [config/types/index.ts:83](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L83)

___

### exclude

• `Optional` `Readonly` **exclude**: *string*[]

Disable formatting for files matching regular expressions. Default to _["node_modules"]_.

Defined in: [config/types/index.ts:27](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L27)

___

### excludeGlob

• `Optional` `Readonly` **excludeGlob**: *string*[]

Disable formatting for files matching glob patterns. Default to _[]_.

Defined in: [config/types/index.ts:31](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L31)

___

### force

• `Optional` `Readonly` **force**: *boolean*

Whether to disregard [exclude](#exclude)/[excludeGlob](#excludeGlob) patterns and file-disable
comments. Default to _false_.

Defined in: [config/types/index.ts:137](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L137)

___

### formatExports

• `Optional` `Readonly` **formatExports**: *boolean*

Whether to format exports as well as imports. Default to _true_.

Defined in: [config/types/index.ts:23](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L23)

___

### groupRules

• `Optional` `Readonly` **groupRules**: (*string* \| *string*[] \| [*GroupRule*](grouprule.md))[]

Grouping rules for path patterns for imports. Default to
[GROUP_RULES_DEFAULT](../README.md#GROUP_RULES_DEFAULT)

**`see`** [Grouping Rules](../../../../wiki/Grouping-Rules)

Defined in: [config/types/index.ts:41](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L41)

___

### hasSemicolon

• `Optional` `Readonly` **hasSemicolon**: *boolean*

Whether to add semicolons at the end of declarations. Default to _true_.

Defined in: [config/types/index.ts:119](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L119)

___

### ignoreESLintRules

• `Optional` `Readonly` **ignoreESLintRules**: *string* \| *string*[]

Ignore ESLint rules matching regular expressions. Default to _[]_.

Defined in: [config/types/index.ts:132](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L132)

___

### insertFinalNewline

• `Optional` `Readonly` **insertFinalNewline**: *boolean*

Whether to end files with a new line. Default to _true_.

Defined in: [config/types/index.ts:123](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L123)

___

### keepUnused

• `Optional` `Readonly` **keepUnused**: [*KeepUnusedRule*](../README.md#keepunusedrule)[]

By default all unused imports are removed. Keep some or all of them around with this setting
if you need.

Defined in: [config/types/index.ts:79](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L79)

___

### maxLineLength

• `Optional` `Readonly` **maxLineLength**: *number*

Max line length before wrapping. 0 for no limit. Default to _80_.

Defined in: [config/types/index.ts:99](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L99)

___

### quoteMark

• `Optional` `Readonly` **quoteMark**: ``"single"`` \| ``"double"``

Use single or double quotes. Default to _single_.

Defined in: [config/types/index.ts:111](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L111)

___

### removeLastIndexInPath

• `Optional` `Readonly` **removeLastIndexInPath**: *boolean*

Whether to remove the last 'index' when normalizing paths. Default to _false_.

Defined in: [config/types/index.ts:95](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L95)

___

### removeLastSlashInPath

• `Optional` `Readonly` **removeLastSlashInPath**: *boolean*

Whether to remove the last slash when normalizing paths. Default to _false_.

Defined in: [config/types/index.ts:91](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L91)

___

### sortImportsBy

• `Optional` `Readonly` **sortImportsBy**: ``"paths"`` \| ``"names"``

Sort import declarations by paths or first names. Default to _paths_.

Defined in: [config/types/index.ts:35](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L35)

___

### sortRules

• `Optional` `Readonly` **sortRules**: ``"none"`` \| [*SortRules*](sortrules.md)

Sorting rules for paths and names. Default to:

```json
{
  "paths": ["_", "aA"],
  "names": ["_", "aA"]
}
```

If it's _none_, then there is no sorting in all groups, unless they have their own
[sort](grouprule.md#sort) defined.

**`see`** [Sorting rules](../../../../wiki/Sorting-Rules)

Defined in: [config/types/index.ts:57](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L57)

___

### tabSize

• `Optional` `Readonly` **tabSize**: *number*

Number of spaces to replace a TAB. Default to _2_.

Defined in: [config/types/index.ts:107](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L107)

___

### tabType

• `Optional` `Readonly` **tabType**: ``"space"`` \| ``"tab"``

Indent lines with tabs or spaces. Default to _space_.

Defined in: [config/types/index.ts:103](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L103)

___

### trailingComma

• `Optional` `Readonly` **trailingComma**: ``"none"`` \| ``"multiLine"``

When to add a trailing comma for the last name. Default to _multiLine_.

Defined in: [config/types/index.ts:115](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L115)

___

### wrappingStyle

• `Optional` `Readonly` **wrappingStyle**: [*WrappingRule*](wrappingrule.md) \| ``"prettier"``

When and how to wrap a line. Default to:

```json
{
  "maxBindingNamesPerLine": 1,
  "maxDefaultAndBindingNamesPerLine": 2,
  "maxExportNamesPerLine": 0,
  "maxNamesPerWrappedLine": 1,
  "ignoreComments": false
}
```

If it's set to _prettier_, then wrap lines in compatible with [Prettier](https://prettier.io/).

**`see`** [Line Wrapping Style](../../../../wiki/Line-Wrapping-Style)

Defined in: [config/types/index.ts:74](https://github.com/daidodo/format-imports/blob/632d67d/src/lib/config/types/index.ts#L74)
