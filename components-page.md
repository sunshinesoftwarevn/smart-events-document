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

**HOW TO USE**

![How to use table](/assets/images/use-table.png)

## Animated Numbers
Animated random number code is a type of code that generates and displays a random number in an animated fashion

|      Properties       |              Type              |    Default Value     | Description                                                                                                                                                                                                                                                                                               |
| :-------------: | :----------------------------: | :------------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| animateToNumber |             number             |      none      | Number to be animated                                                                                                                                                                                                                                                                                     |
|    fontStyle    |      React.CSSProperties?      |      none      | Style of number text                                                                                                                                                                                                                                                                                      |
|  includeComma   |            boolean?            |     false      | Whether the number contains commas                                                                                                                                                                                                                                                                        |
| locale          |           string?              |    en-US       | Formats animated number as per locale. Also it should be used with `inculdeComma` prop. For list of locales, search for "BCP 47 language tags"   |
|   configs(1)    |        SpringConfig[]?         | config.default | This module is using [react-spring](https://www.react-spring.io) and you can refer to this [config option](https://react-spring.io/common/configs). If you pass multiple settings, an animation is randomly assigned to each number. _ DO NOT USE `duration` because of a bug that hasn't been fixed yet_ |
|   configs(2)    | (number, number): SpringConfig | none | The first parameter gives information about the number to be changed, And the second parameter gives information about the order of the changing numbers. You can use that information to adjust the animation by returning the config                                                                    |


## Breadcrumb
Breadcrumb code is a type of markup that helps users navigate through a website. It consists of a list of links that show the user's current location within the site hierarchy.

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| title                     | string     | *undefined*    | Title of breadcrumb        |
| subtitle                     | subtitle     | *undefined*    | Text below title        |
| items                     | Array      | *undefined*    | List breadcrumb        |
| children                     | `ReactNode`      | *undefined*    | React Node children inside breadcrumb       |

**HOW TO USE**

![How to use Breadcrumb](/assets/images/use-breadcrumb.png)

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