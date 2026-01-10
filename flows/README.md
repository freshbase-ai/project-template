# Flows

This directory documents business flows that span multiple modules
or contexts (cross-cutting concerns).

## Suggested Structure

Each flow is a markdown file following the `flow.md` template:

- `onboarding.md` - Customer onboarding flow
- `activation.md` - Service activation flow
- `cancellation.md` - Cancellation flow
- `portability.md` - Number portability flow

## When to Create a Flow

Create a flow document when:
1. The process involves **2+ modules/contexts**
2. There is **orchestration** between systems
3. The flow has defined **states** and **transitions**
4. There are **failure points** that need handling

## Template

Use the `.freshbase/templates/flow.md` template for new flows:

```bash
cp .freshbase/templates/flow.md flows/new-flow.md
```

## Relationship with Other Folders

```
flows/                <- Cross-cutting flows (you are here)
  |
overview/             <- Project overview
  |
.freshbase/contexts/  <- Details of each module involved
```
