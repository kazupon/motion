# useMotionVariants

useMotionVariants is used to handle the [**Variants**](/variants) **state** and **selection**.

## Parameters

### `variants`

A [**Variants**](/variants#custom-variants) definition.

## Exposed

### `state`

The **current** variant **data** value as a **computed**.

### `variant`

A **string** reference that **updates** the state when **changed**.

#### Example

```typescript
const variants: MotionVariants = {
  initial: {
    opacity: 0,
    y: 100,
  },
  enter: {
    opacity: 1,
    y: 0,
  },
}

const { variant, state } = useMotionVariants(variants)

variant.value = 'initial'

nextTick(() => (variant.value = 'enter'))
```
