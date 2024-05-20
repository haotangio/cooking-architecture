---
sidebar_position: 1
---

# Frontend Characteristics

## Framework locked-in

- Unlike backend system, frontend system is more locked-in to the framework. E.g: If you develop iOS native app, you are
  locked-in to Swift or Objective-C with respective SDKs. That's same for Android native app with Java or Kotlin. If you
  develop web app, you are locked-in to React, Angular, Vue, etc.
- It's meaningless to try encapsulate the frontend framework. It's like trying to encapsulate the language itself.

## Backend stability

- Backend APIs are assumed to be stable. If the backend APIs are not stable like introducing API changes without
  backward-compatibility, the frontend will break.
- This is especially true for mobile apps or desktop apps, if the backend changes and breaks the backward compatibility,
  the app will break.

## Volatile and heavy UI/UX

- Requirement changes will affect the UI/UX. This is something we can't resist.
- A lot of development effort fall into building UI components, animations, etc.
- UI components can be heavy, complex, fat and hard to maintain if they're not organized properly.

## Design System consistency

- Even for different kinds of apps across different platforms, the design system should be consistent. E.g: The color,
  typography,
  spacing, etc. should be consistent.

## Clear domain boundary

- The "UI - service - data" aspects of a module is highly coupled and almost like 1 - 1 - 1 mapping.
    - It's unlikely you can reuse the `loginWithEmailAndPassword()` service somewhere else except the `LoginForm`
      component. And you should never try to do that.
- Project Management module should never call APIs of CRM module directly and vice-versa.

```tsx title="LoginForm.tsx"
function LoginForm() {
  const {loginWithEmailAndPassword} = useAuthActions();

  return (
    <Form onSubmit={loginWithEmailAndPassword}>
      <Input type="email"/>
      <Input type="password"/>
      <Button type="submit" label="Login"/>
    </Form>
  );
}
```
