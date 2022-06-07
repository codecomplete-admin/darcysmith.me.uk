---
title: "Starting a technology blog on a budget"
header:
  teaser: "assets/images/markup-syntax-highlighting-teaser.jpg"
categories:
  - Blog
tags:
  - jekyll
  - github pages
  - docker
  - blog
toc: true

---

I've been involved in the software business for over 20 years now. I've learnt a lot and grown a lot in that time...I have the grey hairs to prove it! But, it is only now in May 2022, that I decided the time has come to create my own blog.

## Project: My first blog

There is a short criteria I wanted to meet when starting this blog:

1. It has to be cheap to maintain
2. It has to give a little bit back to all the blogs that I have used in the past to formulate my own solutions to real-world problems
3. Easy to update, easy to deploy. I want to also see my changes locally, before I commit them
4. Feature rich with tagging, categories, search facilities etc
5. Did I say cheap? 

Given this criteria, and a little bit of research into options, I decided that [GitHub Pages](https://pages.github.com/){:target="_blank"} provided me with the perfect platform. In the most part, because GitHub Pages is:

1. Totally free. You get one site per GitHub account and unlimited project sites
2. CMS driven using the [Jekyll](https://jekyllrb.com/) as the static site generator
3. Version controlled - all your content and assets are checked into GitHub each time you make a change
4. Easy to get a feature rich blog in next to time using [Jekyll Themes](https://jekyllrb.com/docs/themes/) with a very active community of Themes to choose from.
5. GitHub also supports [Custom Urls](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) so you can register your own domain name and DNS route through to GitHub - including [securing your site with its very own SSL Certificate](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https) which is also for free!

It's not often that everything lands jam-side-up in life, but this is definitely one of them times...**so what's stopping you from creating your own blog?** Especially that I am going to walk and talk you through how I set mine up...what you waiting for?

## Approach
There is already great documentation available from GitHub on [getting started with HitHub pages](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages), but I wanted a different approach. I want to be able to develop my Jekyll blog locally on my machine, view the changes as I edit them, before I commit them to GitHub and publish them to the outside world.

So in order to get my local Windows machine ready blog development, [Jekyll also has great documentation on getting started locally](https://jekyllrb.com/docs/) too, but I didn't want the faff of installing Ruby, RubGems etc. So instead I'm going to host my Jekyll site locally within a Docker container. 

The Docker container itself will have all the prerequisites to run and server a Jekyll site, and it will expose the port 4000 so I can access it in a browser on my local machine. In my opinion, as I already have Docker installed on my PC for development work anyway, this will prove a much better solution for me.

## Overview

This blog is part of a mult-part series

1. Starting a technology blog on a budget
2. Registering my domain names using AWS Route53
3. Creating an email address for my custom domain and configuring Google mail as my client
4. Create a GitHub account and setup GitHub pages
5. Setup Jekyll site and using Minimal Mistakes theme
6. Running Jekyll using Docker and deployment to GitHub
7. Setting up disqus commenting
8. Creating my first post (this one!)