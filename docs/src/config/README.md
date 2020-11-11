---
sidebar: auto
---

# Config

## foo

- Type: `string`
- Default: `/`

### foo too

## bar

- Type: `string`
- Default: `/`


``` html
<div class="container flex column">
    <TheHeader/> 
    <div>
      <h1 class="title">
        {{page.title}}
      </h1>
      <p>
        {{page.description}}
      </p>
      <nuxt-content :document="page"/>
      <p>
        {{page.under}}
      </p>
    </div>
  </div>
```