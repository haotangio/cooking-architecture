---
sidebar_position: 1
---

# Layer Architecture

## Utilities

Similar to gas and electricity in a house, utilities are the basic services that power the app. They are the building
blocks that are used by the other layers.

Encapsulates:

- **Unit**: Date time, person name, nationality, gender, currency, etc.
- **Validation**: Email, phone, credit card, etc.
- **Formatting**: Date, number, currency, etc.
- **Conversion**: Date to string, string to date, etc.
- **Notification**: Push notification on browsers or mobile devices.
- **Storage**: Local storage, session storage, cookies, etc.
- **Logging**: Log messages to the console or a server.
- **Analytics**: Track user behavior.

## Raw materials

### Design System (@libs/design-system)

Encapsulates:

- **Design Tokens**: Colors, typography, spacing, etc.
- **Components**: Reusable UI components
- **Layouts**: Reusable page layouts
- **Themes**: Light, dark, etc.
- **Utils**: Utility functions
- **Hooks**: Custom hooks
- **Contexts**: React contexts
- **Styles**: Global styles
- **Branding**: Logos, icons, etc.

### Data Layer (@libs/data)

Encapsulates:

- **APIs**: REST, GraphQL, etc.
- **Services**: Business logic
- **Models**: Data structures
- **Stores**: State management
- **Utils**: Utility functions
- **Hooks**: Custom hooks
- **Contexts**: React contexts

## Key Material Layer (@libs/project, @libs/auth, @lib/crm)

Encapsulates:

- **Feature UI components**: Project card, project gantt chart, CRM ticket form, etc.
- **Feature business logic**: Project creation, project update, CRM ticket creation, etc.
- **Feature state management**: Project state, CRM ticket state, etc.
- **Feature data access**: Project data fetching, CRM ticket data fetching, etc.

# Visualizing the layers

[Layer Architecture in Mermaid Chart](https://mermaid.live/view#pako:eNqNlF1v0zAUhv-KZWlcpaNxm64xEmKw202IDZBIduElJ62ZYwfbbSnb_jv-WFmasY-oSk7P--ac5PGJb3ClasAUj0ajUlpuBVD0Ha5Y16E1hw2qoRJMM8uVLGUwNUJtqiXTFl18LCVyh3MYcwINWlkuuN2ihgtBOy6vk0oJpelmyS28G5g120TjQsP2OeM13FdUmskFDKzRfHCAPgh-Zd7GR-BgYt6srhaadUv0dT_vD2dNiy9g7CclJVRW6cs9kRTHkomt5ZXZFybFmbK84VXA4sUHOTx1KJ34Ev402XGJLpB176k9hZZZ0JwJM3iXGgxfyJHZGgtt1Jw9LU5CHp2H_GWPVpD9qdfA03uqAVvZ5YCTs6fFscv3XtnnTt2YCFPEy0A7B73mFZhiFwx0x9fCb2uKXfBIbzslQQbHLhx4ztiaLwLv4iEceC7cfBgRF6Xo_xn4jo0B1yteLv-3KhFPp9VPNxePCZHic5T2C5NnIJEXIJEXIJFXQCKvgEReCYk8CckH_ZnzRBN_h496DKFpMjQavffBzAe337hyvcDcIg2_Mkopl2smeO1y93VDGX-PL_ovlaI3D4of8VLiBLegW8Zrt3fdeGeJ7RJaKDF1YQ0NWwlb4lLeOaubc3W-lRWmVq8gwavO9zzhzK1oi2njvgyX7ZjE9Ab_xpSMp4d5fpRnOZn6XzpL8BbT_HAyScfzCcmyeT7Pj-Z3Cf6jlKuQHo7zWTaek9k0m6YzMgvVfgQttoSauw3mNG62Yc-9-wtHvccT)