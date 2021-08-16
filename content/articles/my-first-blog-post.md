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