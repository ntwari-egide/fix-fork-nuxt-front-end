---
title: My first Blog Post
description: Learning how to use @nuxt/content to create a blog
img: first-blog-post.jpg
alt: my first blog post
---

# Lorem ipsum dolor sit amet consectetur adipisicing elit

Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde voluptatum magni quam numquam distinctio quas minima molestias voluptas aut. Corporis facere, eius rerum veniam asperiores delectus non similique repellendus ipsa!

Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde voluptatum magni quam numquam distinctio quas minima molestias voluptas aut. Corporis facere, eius rerum veniam asperiores delectus non similique repellendus ipsa!

```js
export default {
 nuxt: 'is the best'
}
```

# Lorem ipsum dolor sit amet consectetur adipisicing elit. 
Unde voluptatum magni quam numquam distinctio quas minima molestias voluptas aut. Corporis facere, eius rerum veniam asperiores delectus non similique repellendus ipsa!


Unde voluptatum magni quam numquam distinctio quas minima molestias voluptas aut. Corporis facere, eius rerum veniam asperiores delectus non similique repellendus ipsa!

```vue
<template>
    <div>
        <nuxt-link :to=" 'jokes/'+id ">
            <div class="joke border my-4 p-2">
                <p>{{ joke }}</p>
            </div>
        </nuxt-link>
    </div>
</template>

<script>
export default {
    name: 'Joke',
    props: ['joke','id']
}
</script>

<style>

</style>

```
# Responsive Navbar

[![Netlify Status](https://api.netlify.com/api/v1/badges/b428a366-080f-4668-9ee0-3c6b0ce83d8d/deploy-status)](https://app.netlify.com/sites/nuxt-tailwind-navbar/deploys)

> Beautiful responsive navbar for all your project using [Nuxt.js](https://nuxtjs.org/) and [Tailwind.css](https://tailwindcss.com/)

<p align="center"><img src="../assets/images/post-type.jpg"/></p>
<p align="center"><a href="https://nuxt-tailwind-navbar.netlify.app/">demo</a></p>

## How to run and build the project

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

## Credit

To create this project, I was helped by the work of
- [fayazara](https://github.com/fayazara/tailwind-components)
- [mr_alaraj](https://tailwindcomponents.com/component/traveler-hero-concept-design)
