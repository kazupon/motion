# Quick Start

Let's **get started** quickly by **installing** the **package** and adding the **plugin**.

From your **terminal**:

```bash
yarn add @vueuse/motion
```

In your **Vue** app **entry** file:

```javascript
import { createApp } from 'vue'
import { MotionPlugin } from '@vueuse/motion'
import App from './App.vue'

const app = createApp(App)

app.use(MotionPlugin)

app.mount('#app')
```

You can now **animate** any of your **component**, **HTML** or **SVG** elements using `v-motion`.

```vue
<template>
  <div
    v-motion
    :initial="{
      opacity: 0,
      y: 100,
    }"
    :enter="{
      opacity: 1,
      y: 0,
    }"
  />
</template>
```

To see more about how to use **directives**, check out [**Directive Usage**](/directive-usage).

To see more about what **properties** you can **animate**, check out [**Motion Properties**](/motion-properties).

To see more about how to **create** your own **animations** styles, check out [**Transition Properties**](/transition-properties).

To see more about what are **variants** and how you can **use** them, check out [**Variants**](/variants).

To see more about how to **control** your declared **variants**, check out [**Motion Instance**](/motion-instance).
