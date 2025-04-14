---
sidebar_position: 1
---

# Architecture

| Module types | In cooking                                                      | In application                                      | Notes                  |
|--------------|-----------------------------------------------------------------|-----------------------------------------------------|------------------------|
| Utility      | Gas, water, electricity, etc.                                   | API access, logging, analytics, cookie access, etc. | Don't eat              |
| Common       | Pork, beef, salmon, flour, sugar, salt, pepper, etc.            | Row 2, Col 3                                        | Don't eat              |
| Main         | Pizza, cooked beef, soup, etc.                                  | Row 3, Col 3                                        | Don't eat stealthily   |
| App          | Well decorated ready-to-eat meals: Pizza dish, Pho's bowl, etc. | Webpage with URL, modal, mobile app screen          | Enjoy the meal         |

## Utility module

Similar to kitchen facilities: gas, electricity, water, ... - which are well-prepared by the kitchen staffs and are
ready to be used by the chefs.
It's something that the diners don't care about but the chef does.
In the frontend system, the utility module is like a set of utilities that are well-prepared and ready to be used by the
feature modules.

> The diners don't "eat" the gas, electricity, or water. Similarly, the users don't use the utility module directly.
>
> Look at the gas, electricity, water, ... of a kitchen. You can't predict what kind of dish will be cooked in the
> kitchen. Similarly, the utility module is not aware of what kind of application it is used in.

Encapsulates:

- **Unit**: Date time, nationality, gender, currency, etc.
- **Validation**: Email, phone, credit card, etc.
- **Formatting**: Date, number, currency, etc.
- **Conversion**: Date to string, string to date, etc.
- **Notification**: Push notification on browsers or mobile devices.
- **Storage**: Local storage, session storage, cookies, etc.
- **Logging**: Log messages to the console or a server.
- **Analytics**: Track user behavior.
- **Network connector**: Connector like Axios, Fetch, etc.

## Common module

Common module are like uncooked raw material and ingredients: pork, beef, salmon, flour, sugar, salt, pepper, ... -
which are used by the chefs to cook the dishes.
In the application, the common module is like a set of common functionalities that are used by the feature modules.

> In most of the time, diners don't eat the raw material and ingredients directly (except Sashimi ^^). Similarly, the
> users don't use the common module directly.
>
> Look at the pork, beef, salmon, flour, sugar, ... you can't confidently predict what exact dish will be cooked.
> Similarly, the common module is not aware of what exact of application it is used in.

Encapsulates:

- **Design System**:
  - **Design Tokens**: Colors, typography, spacing, etc.
  - **Components**: Reusable UI components
  - **Layouts**: Reusable page layouts
  - **Themes**: Light, dark, etc.
  - **Contexts**: React contexts
  - **Styles**: Global styles
  - **Branding**: Logos, icons, etc.
- **Error Handling**
- **Internationalization**:
    - **Translations**: Language translations
    - **Localization**: Date, number, currency, etc.
- **Authentication**:
  - **Authentication UI**: Login screen or modal.
  - **Auth context**: Access to current login user value and other helpers.
- **Authorization**:
  - **Access protection mechanic**: Prevent users access certain features, using modal or screen redirection.

## Main module

Main module is where the main material of the dish is cooked: pizza dough, beef tomato sauce, ...
In the application, the main module is where the main functionalities of the application are implemented.

> If you're familiar with Domain Driven Design, imagine the main module as the "Core Domain" of the application which
> includes a cluster of "Aggregate Roots".

Encapsulates:

- **Feature UI components**: Project card, project gantt chart, CRM ticket form, etc.
- **Feature business logic**: Project creation, project update, CRM ticket creation, etc.
- **Feature state management**: Project state, CRM ticket state, etc.
- **Feature navigation**: URLs or screen names of feature models like edit project info, view task ticket, etc.
- **Feature data model**: Project model, task model, etc.
- **Feature data access**: Project data fetching, CRM ticket data fetching, etc.

## App module

Encapsulates:

- **Feature UI components**: Project card, project gantt chart, CRM ticket form, etc.
- **Feature business logic**: Project creation, project update, CRM ticket creation, etc.
- **Feature state management**: Project state, CRM ticket state, etc.
- **Feature data access**: Project data fetching, CRM ticket data fetching, etc.

# Visualizing the layers

[Layer Architecture in Mermaid Chart](https://mermaid.live/view#pako:eNqNlF1v0zAUhv-KZWlcpaNxm64xEmKw202IDZBIduElJ62ZYwfbbSnb_jv-WFmasY-oSk7P--ac5PGJb3ClasAUj0ajUlpuBVD0Ha5Y16E1hw2qoRJMM8uVLGUwNUJtqiXTFl18LCVyh3MYcwINWlkuuN2ihgtBOy6vk0oJpelmyS28G5g120TjQsP2OeM13FdUmskFDKzRfHCAPgh-Zd7GR-BgYt6srhaadUv0dT_vD2dNiy9g7CclJVRW6cs9kRTHkomt5ZXZFybFmbK84VXA4sUHOTx1KJ34Ev402XGJLpB176k9hZZZ0JwJM3iXGgxfyJHZGgtt1Jw9LU5CHp2H_GWPVpD9qdfA03uqAVvZ5YCTs6fFscv3XtnnTt2YCFPEy0A7B73mFZhiFwx0x9fCb2uKXfBIbzslQQbHLhx4ztiaLwLv4iEceC7cfBgRF6Xo_xn4jo0B1yteLv-3KhFPp9VPNxePCZHic5T2C5NnIJEXIJEXIJFXQCKvgEReCYk8CckH_ZnzRBN_h496DKFpMjQavffBzAe337hyvcDcIg2_Mkopl2smeO1y93VDGX-PL_ovlaI3D4of8VLiBLegW8Zrt3fdeGeJ7RJaKDF1YQ0NWwlb4lLeOaubc3W-lRWmVq8gwavO9zzhzK1oi2njvgyX7ZjE9Ab_xpSMp4d5fpRnOZn6XzpL8BbT_HAyScfzCcmyeT7Pj-Z3Cf6jlKuQHo7zWTaek9k0m6YzMgvVfgQttoSauw3mNG62Yc-9-wtHvccT)
