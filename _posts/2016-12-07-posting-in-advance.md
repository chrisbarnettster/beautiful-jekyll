---
layout: post
title: Jekyll drafts and future posts
subtitle: 'use _drafts or hidden: true'
bigimg: /img/LEGO-sustainable-building-brick_trimmed.jpg
tags: [jekyll, drafting]
---

Without reading too much documentation I thought creating a future dated post would be a great way to start drafts and then 'autopublish' posts.

Don't do that rather use the standard jekyll draft mechanism!

As it happen,  my local jekyll docker honors the future dated post idea but github.io still renders future posts.

I am using the Pagination gem and [Pagination pages through every post in the posts variable unless a post has hidden: true in its YAML Front Matter.](https://jekyllrb.com/docs/pagination/)

# Using jekyll's draft mechanism

This works well.

- create a drafts post in \_drafts folder in your site’s root.
- Serve jekyll with the --drafts flags e.g. `jekyll serve --force_polling --drafts`
- Current drafts show up as latest posts.
- When ready to publish move the draft to \_posts/YYYY-MM-DD-new-post.md

This is described [here](https://jekyllrb.com/docs/drafts/) and really well explained [here](http://hamishwillee.github.io/2014/06/11/public-drafts-in-jekyll/)

# Future posts  - Use hidden: true

Using "hidden: true" is a poor replacement for the drafts mechanism. However, it is may be useful for keeping prepared future posts hidden.

For example a future dates post \_posts/3016-12-31-future-post.md would include the following YAML frontmatter:

```
---
layout: post
title: Very much a future post
hidden: true
---
```

Credits: [pic](http://inhabitat.com/lego-just-invested-150-million-to-make-a-better-more-sustainable-building-brick/)
