---
title: 'My First Blog with Astro'
description: 'Discovering Astro and building my personal tech blog from scratch'
author: 'Shrinandana'
pubDate: 'Feb 10 2026'
heroImage: '../../assets/blog-placeholder-3.jpg'
---

## Introduction

When I decided to start my personal tech blog, I knew I wanted something fast, modern, and beginner-friendly. That's when I discovered **Astro**, and it completely changed how I think about building web projects.

In this post, I'll share my journey of creating this very blog, why I chose Astro, and the key lessons I learned along the way.

## What is Astro?

Astro is a modern static site builder that lets you build web applications using your favorite frameworks (React, Vue, Svelte, etc.) while sending minimal JavaScript to users. Here's what makes it special:

**Zero JavaScript by Default**: Astro sends HTML and CSS to the browser without unnecessary JavaScript, making your sites incredibly fast.

**Component-Driven**: You can use components from different frameworks in the same project. Need a React component here and a Vue component there? Astro handles it seamlessly.

**Content-First**: Astro was built with content creators in mind. It has built-in support for Markdown and content collections, making it perfect for blogs.

**Great Performance**: Since Astro generates static HTML at build time, your blog loads lightning-fast.

## Why I Chose Astro

Before settling on Astro, I considered several options:

- **Blogger/Medium**: Simple, but limited customization
- **Next.js**: Powerful, but felt like overkill for a static blog
- **Hugo**: Fast, but the learning curve wasn't ideal for someone new to static site generators
- **Astro**: The perfect balance of simplicity and power

What convinced me was Astro's focus on **content and performance**. It treats blog posts as first-class citizens, has excellent documentation for beginners, and the developer experience is fantastic.

## How I Created This Blog

### Step 1: Setting Up the Project

I started by creating a new Astro project using the CLI:

```bash
npm create astro@latest my-blog
cd my-blog
npm run dev
```

The setup wizard guided me through choosing a starter template. I selected the blog template, which came with essential files like pages, layouts, and components already set up.

### Step 2: Understanding the Project Structure

The blog template provided a clear structure:

```
src/
├── content/
│   └── blog/          # My blog posts live here
├── pages/
│   ├── index.astro    # Home page
│   └── blog/
│       ├── index.astro    # Blog listing page
│       └── [...slug].astro # Dynamic blog post page
├── components/        # Reusable components
├── layouts/          # Layout templates
└── styles/           # Global styles
```

### Step 3: Creating Blog Posts

The easiest part! I created a new Markdown file in `src/content/blog/`:

```markdown
---
title: 'My Post Title'
description: 'A short description'
author: 'Shrinandana'
pubDate: 'Feb 10 2026'
heroImage: '../../assets/image.jpg'
---

## Markdown Content Here

You can use **bold**, *italics*, and all standard Markdown syntax!
```

That's it! Astro automatically converts each Markdown file into a blog post page.

### Step 4: Customizing Look and Feel

The starter came with beautiful components like headers, footers, and post cards. I tweaked the styles to match my personal brand without changing the overall structure.

## Key Lessons Learned

### 1. Content Collections Make Everything Easier

Astro's content collections feature automatically validates your blog post frontmatter against a schema. This caught mistakes early and ensured consistency across all posts.

### 2. Markdown is Perfect for Blogging

Writing content in Markdown is fast and distraction-free. No complex editors needed—just plain text with simple formatting.

### 3. Static Generation is Powerful

Since Astro builds your entire blog at build time, there's no database to maintain, no server to manage. Just pure HTML, CSS, and minimal JavaScript. This makes deployment simple and keeps performance stellar.

### 4. Astro's Documentation is Beginner-Friendly

When I got stuck, the official Astro docs had clear examples and explanations. The community is welcoming and helpful too.

## What's Next?

Now that my blog is up and running, I'm excited to:

- Write more posts sharing my learning journey
- Experiment with Astro's advanced features
- Connect with other developers in the Astro community
- Share my experiences learning web development

## Conclusion

Starting this blog with Astro was one of the best decisions I've made as a beginner web developer. It taught me about static site generation, modern web performance, and the importance of choosing the right tool for the job.

If you're thinking about starting a blog or building a fast, content-heavy website, I highly recommend giving Astro a try. It's beginner-friendly, well-documented, and genuinely fun to work with.

Happy blogging! 🚀
