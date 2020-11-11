---
home: true
# heroImage: https://ik.imagekit.io/alexborecky/shoptetak/chat_1HWUbvPEg.png
# tagline: Testing environment of VuePress
# actionText: Quick Start →
# actionLink: /guide/
# features:
# - title: Feature 1 Title
#   details: Feature 1 Description
# - title: Feature 2 Title
#   details: Feature 2 Description
# - title: Feature 3 Title
#   details: Feature 3 Description
footer: Made by Alex with ❤️
---

<h2> Templates </h2>
<div class="products">
  <PreviewComponent
      v-for="item in templates" 
      :key="item.title" 
      :to="item.link"
      :productTitle="item.title"
      :productImage="item.image"
      :productLink="item.link"
      :productDescription="item.description"
    />
</div>

<h2> Addons </h2>
<div class="products">
  <PreviewComponent
      v-for="item in addons" 
      :key="item.title" 
      :to="item.link"
      :productTitle="item.title"
      :productImage="item.image"
      :productLink="item.link"
      :productDescription="item.description"
    />
</div>



<script>
export default {
  data() {
    return {
      templates: [
        {
          title: 'Product one', 
          link: '/product-one', 
          image: 'https://ik.imagekit.io/alexborecky/shoptetak/Doplnky/pop-up_IrWaPVVkMY.png',
          description: 'This is a short description of the product'
        },
        {
          title: 'Product two', 
          link: '/product-one', 
          image: 'https://ik.imagekit.io/alexborecky/shoptetak/Doplnky/pop-up_IrWaPVVkMY.png',
          description: 'This is a short description of the product'
        },
        {
          title: 'Product three', 
          link: '/product-one', 
          image: 'https://ik.imagekit.io/alexborecky/shoptetak/Doplnky/pop-up_IrWaPVVkMY.png',
          description: 'This is a short description of the product'
        },
        {
          title: 'Product four', 
          link: '/product-one', 
          image: 'https://ik.imagekit.io/alexborecky/shoptetak/Doplnky/pop-up_IrWaPVVkMY.png',
          description: 'This is a short description of the product'
        },
      ],
      addons: [
        {
          title: 'Addon one', 
          link: '/product-one', 
          image: 'https://ik.imagekit.io/alexborecky/shoptetak/Doplnky/pop-up_IrWaPVVkMY.png',
          description: 'This is a short description of the Addon'
        },
        {
          title: 'Addon two', 
          link: '/product-one', 
          image: 'https://ik.imagekit.io/alexborecky/shoptetak/Doplnky/pop-up_IrWaPVVkMY.png',
          description: 'This is a short description of the Addon'
        },
      ]
    }
  }
}

</script>

<style lang="scss" scoped>

.products {
  display: flex;
  flex-wrap: wrap;
  margin: 16px -40px;
}

.products > * {
  flex: 0 0 264px;
  margin: 16px 40px;
  @media only screen and (max-width: 960px){
    flex: 0 0 160px;
  }
}

</style>