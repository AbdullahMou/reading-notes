# react IV:

## Data Fetching

* **Pre-rendering.**
  * Each generated HTML is associated with minimal JavaScript code necessary for that page.
  * When a page is loaded by the browser, its JavaScript code runs and makes the page fully interactive. 
  * **Static Generation**
    * is the pre-rendering method that generates the HTML at build time. The pre-rendered HTML is then reused on each request.
  * **Server-side Rendering**
    * is the pre-rendering method that generates the HTML on each request.

## Dynamic Routes

### Statically Generate Pages with Dynamic Routes

* In our case, we want to create dynamic routes for blog posts:

  * We want each post to have the path /posts/<id>, where <id> is the name of the markdown file under the top-level posts directory.
  * Since we have ssg-ssr.md and pre-rendering.md, we’d like the paths to be /posts/ssg-ssr and /posts/pre-rendering.

### Implement getStaticPaths
* First, let’s set up the files:

  * Create a file called [id].js inside the pages/posts directory.
  * Also, remove first-post.js inside the pages/posts directory — we’ll no longer use this.  

### Implement getStaticProps

* We need to fetch necessary data to render the post with the given id.

  * To do so, open lib/posts.js again and add the following getPostData function at the bottom. It will return the post data based on id  

### Render Markdown
* To render markdown content, we’ll use the remark library. 
* open lib/posts.js and add import remark and html
* And update the getPostData() function


## Deploying Your Next.js App

### Deploy to Vercel

* The easiest way to deploy Next.js to production is to use the Vercel platform developed by the creators of Next.js.

* Vercel is an all-in-one platform with Global CDN supporting static & JAMstack deployment and Serverless Functions. We believe Vercel is the optimal place to deploy Next.js apps. 

  * Pages that use Static Generation and assets (JS, CSS, images, fonts, etc) will automatically be served from the Vercel Edge Network, which is blazingly fast.
  * Pages that use Server-Side Rendering and API routes will automatically become isolated Serverless Functions. This allows page rendering and API requests to scale infinitely.
* Vercel has many more features, such as:

  * Custom Domains: Once deployed on Vercel, you can assign a custom domain to your Next.js app. Take a look at our documentation here.
  * Environment Variables: You can also set environment variables on Vercel. Take a look at our documentation here. You can then use those environment variables in your Next.js app.
  * Automatic HTTPS: HTTPS is enabled by default (including custom domains) and doesn't require extra configuration. We auto-renew SSL certificates.
  
