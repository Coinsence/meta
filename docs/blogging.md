# Blogging

We will be using a static site generator like **Jekyll**

We have chosen mediumish-theme-jekyll tempalte as a working template for our blog which you can lear more about it [here](https://wowthemesnet.github.io/mediumish-theme-jekyll/about)

## Installing locally

Jekyll is a Ruby Gem that can be installed on most systems.

### Requirements

Requirements are as described on the Jekyll installation docs:  https://jekyllrb.com/docs/installation/#requirements

* Git
* Ruby
* RubyGems
* GCC and Make

You can follow installation guide as prescribed in offical docs: https://jekyllrb.com/docs/installation/#guides

### Running

After making sure all the requirements are set, then you should be able to run your Jekyll site:

1. `git clone https://github.com/Coinsence/coinsence.github.io.git`
2. `cd coinsence.github.io`
3. `bundle`
4. `jekyll serve --watch` or `bundle exec jekyll serve`
6. Some YAML post settings:
    * post image - `image: assets/images/mypic.jpg`
    * external post image - `image: "https://externalwebsite.com/image4.jpg"`
    * page comments - `comments:true`
    * meta description (optional) - `description: "this is my meta description"`

### Posting

You can start adding your **.md** files in **_posts** folder.

#### *Some YAML post settings*

* post image - `image: assets/images/mypic.jpg`
* external post image - `image: "https://externalwebsite.com/image4.jpg"`
* page comments - `comments:true`
* meta description (optional) - `description: "this is my meta description"`


#### *YAML Post Example*

```
---
layout: post
title:  "We all wait for summer"
author: john
categories: [ Jekyll, tutorial ]
image: assets/images/5.jpg
description: "Something about this post here"
rating: 4.5
---

POST CONTENT HERE...
```

### Configuring

You can start configuring the site by modifying the `_config.yml` file.

#### *Authors*

You can add authors in the **authors** section on the aftermentioned file above. An example below:

```
sal:
    name: Sal
    display_name: Sal
    gravatar: e56154546cf4be74e393c62d1ae9f9d4
    email: wowthemesnet@gmail.com
    web: https://www.wowthemes.net
    twitter: https://twitter.com/wowthemesnet
    description: "Author of Mediumish, a Bootstrap Medium styled template available for WordPress, HTML, Ghost and Jekyll. You are currently previewing Jekyll template demo."
```


## Deployment

As Github already supports running Jekyll templates directly without compiling, you can push your modified code and/or newely added posts/pages, and github will take care of the rest! You can learn more about that [here](https://help.github.com/en/articles/using-jekyll-as-a-static-site-generator-with-github-pages).

So just commit, push and profit! :sunglasses: :v:
