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
| api                     | `Functional`      | *undefined*    | Api gets a list to show        |
| defs                    | object          | *undefined*    | Config table of columns via [table antd](https://4x.ant.design/components/table/#Column)        |
| showCheckbox            | boolean         | true           | Config to show or hide a checkbox        |
| showDeleteItem          | boolean         | true           | Config to show or hide a delete action        |
| showPagination          | boolean         | false          | Config to show or hide a pagination        |
| defaultPageSize         | number          | 20             | Limit of list        |
| rowKey                  | string          | "id"           | Key of row        |
| apiDelete               | `Functional`      | *undefined*    | Api functional for delete action        |
| afterDeleteSuccess      | `Functional`      | *undefined*    | Action after delete success        |
| loading                 | boolean         | false          | Loading table        |
| treeMode                | boolean         | false          | Tree mode        |
| scroll                  | object          | Default scroll | Config scroll        |
| modeRowKeys             | object          | *undefined*    |         |
| disableAllCheckbox      | boolean         | false          | Disabled all checkbox        |
| disableCheckboxKey      | boolean         | false          | Disabled all checkbox key        |
| disableCheckboxFunction | boolean         | false          | Disabled all checkbox function        |
| rowKeysChange           | `Functional`      | false          | Handle change keys action        |
| scrollToFirstRowOnChange| boolean         | true           | Scroll to first when row changed        |
| conditionShowDeleteItem | `Functional`      | *undefined*    | Conditional to show delete        |
| customRequestDelete     | object          | *undefined*    | Custom request delete action        |
| bordered                | boolean         | true           | Border of table        |
| customAction            | `Functional`      | *undefined*    | Custom Action of Action columns        |
| showEditItem            | boolean         | false          | Show edit item        |
| editPathRoute           | `Functional`      | *undefined*    | Route or action to edit item       |
| typeAction              | string          | *undefined*    | Type action of action columns         |
| menuAction              | Functional      | *undefined*    | Menu item of action columns        |
| renderAction            | Functional      | *undefined*    |         |
| onGroupRowAction        | Functional      | *undefined*    |         |
| fixedValuesFilter       | object          | *undefined*    | Values filter fixed        |
| searchPlaceHolder       | string          | 'CORE:search_holder'    | Placeholder of search        |
| customRightAction       | `Functional`          | *undefined*    | Right action        |
| customCheckAction       | `Functional`          | *undefined*    | Check action        |
| listFilter       | Array          | *undefined*    | List filter key mapping via filter dynamic        |
| showFilter       | boolean          | false    | Show Filter action        |
| sortPositionName       | string          | 'desc'    | Key of sort        |
| typeSort       | string          | 'sortField'    | Type of sort key        |

HOW TO USE
==========

![How to use table](/assets/images/use-table.png)

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