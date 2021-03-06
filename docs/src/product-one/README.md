# Introduction

[[toc]]

VuePress is composed of two parts: a [minimalistic static site generator](https://github.com/vuejs/vuepress/tree/master/packages/%40vuepress/core) with a Vue-powered [theming system](https://v1.vuepress.vuejs.org/theme/) and [Plugin API](https://v1.vuepress.vuejs.org/plugin/), and a [default theme](https://v1.vuepress.vuejs.org/theme/default-theme-config.html) optimized for writing technical documentation. It was created to support the documentation needs of Vue's own sub projects.

## Subchapter
Each page generated by VuePress has its own pre-rendered static HTML, providing great loading performance and is SEO-friendly. Once the page is loaded, however, Vue takes over the static content and turns it into a full Single-Page Application (SPA). Additional pages are fetched on demand as the user navigates around the site.

### Third layer

This is some more text

::: warning
This is a warning
:::

## Subchapter Two

``` html{6}
<ul>
  <li
    v-for="todo in todos"
    :key="todo.id"
  >
    {{ todo.text }}
  </li>
</ul>
```

<demo-component
    :msg="msg"
/>


<script>
    export default {
        data () {
            return {
                msg: 'This is a different message'
            }
        }
    }

</script>