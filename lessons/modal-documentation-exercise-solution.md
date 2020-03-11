---
path: "/modal-documentation-exercise-solution"
title: "Modal documentation exercise solution"
section: "Documenting components with Storybook"
order: 63
---

```jsx
import { Meta, Story, Preview } from "@storybook/addon-docs/blocks";
import { withKnobs, boolean } from "@storybook/addon-knobs";
import { SignUpModal, SignInModal } from "./Modals";

<Meta title="Design System|Modals" component={SignUpModal} />

# Modals

Modals are dialogs which overlay content to convey.

## Usage

Use modals to call the user to action or complete a task.

## Sign In Modal

The SignInModal is used to prompt the user to sign in to their account.

<Preview withToolbar>
  <Story name="signIn">
    <SignInModal showModal={boolean("Show Modal", true)} />
  </Story>
</Preview>

## Sign Up Modal

The SignUpModal is used to prompt the user to create an account.

<Preview withToolbar>
  <Story name="signUp">
    <SignUpModal showModal={boolean("Show Modal", true)} />
  </Story>
</Preview>
```