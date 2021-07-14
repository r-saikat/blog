# blog
 This is my blog with uBlogger Hugo theme.

### Add authors
data/authors/

Add the details in json format.

Then, visit the home directory and open config.yaml
Change this part:

```
author:
  name: saikat.en
```

### Change Favicon

To change the icon (favicon) displayed next to the title in the browser tab,

  1. Visit [this website](https://realfavicongenerator.net/)
  2. Use the SVG and generate the zip folder
  3. Extract the zip folder to `/static/`.
  
### Drafting a post

If you want to render the post locally but do not want to render it on your public website yet, due to obvious reasons, add `draft: true` in the `YAML` section of the post. After you have finalised the post, change it to `draft: false`.

`publishdate:date-here` in the `YAML` allows you to specify a future publish date of your post

### Expose locally rendered webserver

You may want to test the rendered website on a phone without pushing the site to GitHub. `blogdown::serve_site(host = '0.0.0.0')` enables you to serve our locally rendered website to 0.0.0.0. If you want someone else on the internet to access the website, forward the requisite port in your router's firewall.

### High quality images

Add `knitr::opts_chunk$set(fig.retina = 2)` in an R code chunk (obviously with `echo=FALSE`) to globally enable rendering high quality images in the post.

# Deployed with Netlify

[![Netlify Status](https://api.netlify.com/api/v1/badges/91fd5144-a81a-4cb8-8ba6-965b2ffffabb/deploy-status)](https://app.netlify.com/sites/heuristic-stonebraker-a9704e/deploys)
