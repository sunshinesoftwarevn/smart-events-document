# Components directory

The components directory contains your React.Js Components. Components are what makes up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

___

## Admin Tables
This component is a defined table with fetching data via static structural common for all systems.

![Admin Table Structural](/assets/images/admin-table-structural.png)

The structural structure of these components contains the core table, dynamic filter action, and styles.
To get started, please continue with the **index.js** file.

**Component API:**

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| api                     | `Functional`      | *undefined*    | Notes        |
| defs                    | object          | *undefined*    | Notes        |
| showCheckbox            | boolean         | true           | Notes        |
| showDeleteItem          | boolean         | true           | Notes        |
| showPagination          | boolean         | false          | Notes        |
| defaultPageSize         | number          | 20             | Notes        |
| rowKey                  | string          | "id"           | Notes        |
| apiDelete               | `Functional`      | *undefined*    | Notes        |
| afterDeleteSuccess      | `Functional`      | *undefined*    | Notes        |
| loading                 | boolean         | false          | Notes        |
| treeMode                | boolean         | false          | Notes        |
| scroll                  | object          | Default scroll | Notes        |
| modeRowKeys             | object          | *undefined*    | Notes        |
| disableAllCheckbox      | boolean         | false          | Notes        |
| disableCheckboxKey      | boolean         | false          | Notes        |
| disableCheckboxFunction | boolean         | false          | Notes        |
| rowKeysChange           | `Functional`      | false          | Notes        |
| scrollToFirstRowOnChange| boolean         | true           | Notes        |
| conditionShowDeleteItem | `Functional`      | *undefined*    | Notes        |
| customRequestDelete     | object          | *undefined*    | Notes        |
| bordered                | boolean         | true           | Notes        |
| customAction            | `Functional`      | *undefined*    | Notes        |
| showEditItem            | boolean         | false          | Notes        |
| editPathRoute           | `Functional`      | *undefined*    | Notes        |
| typeAction              | string          | *undefined*    | Notes        |
| menuAction              | Functional      | *undefined*    | Notes        |
| renderAction            | Functional      | *undefined*    | Notes        |
| onGroupRowAction        | Functional      | *undefined*    | Notes        |
| fixedValuesFilter       | object          | *undefined*    | Notes        |

## Breadcrumb
Inside your templates, if you need to link to your assets directory use 

## Animated Numbers

## Camera

## Ckeditor

## ErrorBoundary

## Input Code

## Konva Editor

## Modal Preview

## Modal PIN

## Select Font

## Show More

## Spin & Spinner

## Upload Image