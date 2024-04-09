---
author: bandit
pubDatetime: 2024-04-09T
title: New To Astro
slug: "new-to-astro"
featured: true
ogImage: ../../assets/images/AstroPaper-v4.png
tags:
  - release
description: "New To Astro: how to fastly use astro from a newbie who knows nothing about astro."
---

Hello, this is my first post using astro.

## table of contents

## Background

### Old experience
I have been using WordPress for some years, but not dave deep into it. I used WordPress as blog to writing sometimes, 
as I should have a vps at least, It's a cost for me. So I could not continue all the time.

### Why I Choose Astro?
However, there many free serverless hosting service, they even server you with free domain and free ssl licence,
so I try to write some blogs again. There are  so many free deploy service for astro ,you can use them from [astro docs](https://docs.astro.build/zh-cn/guides/deploy/)

And those many sponsors not only serve Astro, another reason I choose Astro because I want to have a try on SEO, wordPress also
has Astro theme, the first time I heard about Astro is because it's great SEO performance in wordPress. I didn't know
there is a javascript/typescript version.

A better SEO performance also calls for better loading speed, this is also Astro good at.[This is google's lighthouse score for astro and its theme paper.](https://pagespeed.web.dev/analysis/https-astro-paper-pages-dev/hlq7hdrwfk?form_factor=desktop)
![ligthhouse-score-for-astro-paper](@assets/images/ligthhouse-score-for-astro-paper.png)

## how to start

### Tools
you need three tools:

---- A build tool, Node.js(>=v18.14.1) and its package manager npm   
---- A framework, Astro    
---- A Astro theme, I will recommend for [paper](https://github.com/satnaing/astro-paper)    

### prepare for blogging
1. Download Node.js and install it.
2. create a Astro project on theme pager
    ```
    # npm 6.x
    npm create astro@latest --template satnaing/astro-paper
    # npm 7+, extra double-dash is needed:
    npm create astro@latest -- --template satnaing/astro-paper
    # yarn
    yarn create astro --template satnaing/astro-paper
   ```
3. you can use command "npm run dev" to preview your blog in your computer.
    ```
    % npm run dev
    
    > dev
    > astro dev
    
    ▶ Astro collects anonymous usage data.
    This information helps us improve Astro.
    Run "astro telemetry disable" to opt-out.
    https://astro.build/telemetry
    
    19:53:13 [vite] Re-optimizing dependencies because vite config has changed
    
    astro  v4.2.1 ready in 1168 ms
    
    ┃ Local    http://localhost:4321/
    ┃ Network  use --host to expose
    ```
   then open http://localhost:4321/ in your browser, you will see it.
4. connect this code with your GitHub repository, you need to use GitHub to manage your code.
   1. firstly create a repository such as astro_blog
   2. then connect your project with the repository and push your code to the repository
       ```
       git remote add origin https://github.com/banditsmile/astro_blog.git
       git branch -M main
       git push -u origin main
       ```
5. deploy to hosting service( Vercel for example)
   1. create a vercel.com account
   2. connect your github.com account with vercel.com
   3. create a project in vercel.com and choose the repository you just created in GitHub.
