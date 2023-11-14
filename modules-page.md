# Modules

Modules in source code are a way of organizing and structuring code into smaller, reusable units. They can help to improve the readability, maintainability, and testability of code.
___

## Core Structural

### Mapping module

Modules are mapped using keys in the Modules/index.js file

![Mapping modules](/assets/images/mapping-modules.png) 

### assets

Just like the assets of the entire system, this place contains images, svg, fonts and css

### Components

Components used specifically for features on the module will be attached here, such as tables of each feature, management forms,...

### configs

#### api

Contain all API route constants of the module.

#### constants

Contain all constants used for modules.

### i18n -> localization

Includes 2 translation files: en.json and vi.json for translation and common use throughout the system

### Page

It is the outermost main page of a route module

### style
Contain custom CSS style used for modules.

### Store
Includes service (main api) and store redux toolkit declaration

### bootstrap.js

**Example**
![bootstrap of modules](/assets/images/bootstrap-module.png)

***Properties***

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| name                     | string     | *undefined*    | Name of module       |
| dir                     | string     | *undefined*    | Dir name of foler modules      |
| pathRoot                     | object     | *undefined*    | Path root is main route path, example: [domain]/[main]/[url]        |
| routes                     | routes[]     | *undefined*    | List routes       |
| lang                     | Object     | *undefined*    | Define language of module via {vi, en}      |
| isAuthenticate                     | boolean or `Any`    | *undefined*    | Check modules auth or unauth or public      |
| roles                     | string or Array     | *undefined*    | Check roles allow route      |

***Routes Properties***

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| url                     | string     | *undefined*    | Sub url of route       |
| component                     | string     | *undefined*    | Path to Component       |
| meta                     | object     | *undefined*    | Meta of modules route       |
| layout                     | string | `FullLayout` | `BlankLayout`     | `FullLayout`    | Layout of route       |
| props                     | object     | *undefined*    | Props pass to layout      |

## Account 
Manage personal information of organizers

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | Includes operations to edit basic information of the organizers       |

## Authenticate
User identity authentication feature

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Blank Layout                     | undefined    | false   | Login Page       |

## CheckInOut
The user check in and check out feature is reserved for the organizers

Required: `PIN`

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | CheckIn & CheckOut       |

## CheckInOutPublic
The user check in and check out feature is reserved for all user

Required: `PIN`

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Blank Layout                     | undefined     | 'Any'   | CheckIn & CheckOut       |


## DynamicGroupCode
Dynamic code groups are groups of options for user registration forms

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `Admin Super`     | true   | Dynamic code groups       |

## DynamicOption
Dynamic options are the options of dynamic groups for the user registration form

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `Admin Super`     | true   | Options       |

## Event
Manage system events


## Gallery

## GroupInvite
Manage group invite

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | Group customer invite       |

## Home
Dashboard admin will show the welcome banner and btc will show statistics, charts and schedules

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | undefined     | true   | Dashboard admin       |

## InfoEventPayment

Manage and approve registration applications for event organizers

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | Manage and approve registration applications for event organizers      |

## InfoPin

Manage PIN codes for each event

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | Manage and approve registration applications for event organizers      |

## InfoPrizesLuckydraw

Manage PIN codes for each event

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | Manage and approve registration applications for event organizers      |

## LuckyDraw

Lucky dial interface for event btc

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | Lucky Draw     |

## Notification

Manage and push notifications

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | Lucky Draw     |

## NotificationClient

See notification list for btc


Manage and push notifications

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Full Layout                     | `BTC`     | true   | Notification     |

## Public

The system's public pages are for users

| Layout              | Roles           | Auth  | Description  |
| --- |---| ---| ---|
| Blank                     | undefined     | true   | Public Page     |

## Smtp

## UserInvite

## UserRegister
