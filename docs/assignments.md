---
layout: doc
---

<script setup>
  import {data as assign} from './assignments/assignments.data';
  import { withBase } from 'vitepress';
</script>

# Assignments

<ul v-if="assign.length > 0">
  <li v-for="blog of assign">
    <a :href="withBase(blog.url)">{{ blog.frontmatter.title }}</a>
  </li>
</ul>
<p v-else>
  Nothing here yet!
</p>
