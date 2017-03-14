## Features Overview

- Cover image for posts and pages
- Tags Support
- Responsive Images
- Social Accounts configuration
- Pagination

## Not Supported

- Post Categories will not be displayed
- Posts and Pages Dates not displayed anywhere 

## External libraries used

- [jQuery](https://jquery.com/)

## Installation

```
$ git clone https://github.com/klugjo/hexo-theme-magnetic themes/magnetic
```

Then update your blog's main `_config.yml` to set the theme to `magnetic`:

## Theme Configuration

The theme's global configuration is done in `/themes/hexo-theme-magnetic/_config.yml`.

### Menu

The menu is configured in the theme's `_config.yml`.

```
# Header
menu:
  Home: /
  Archives: /archives
```

The object key is the label and the value is the path.

### Default index page cover image

You can specify a default thumbnail for posts on the index page (Home page). This image will be used if you forget to specify an image in the post's front matter.

```
# Default post cover index page
default_cover_index: "http://placehold.it/450x450"
```

### Default post page cover image

You can specify a default thumbnail for posts/pages on the post/page page (Detail Page). This image will be used if you forget to specify an image in the post's front matter.

### Default post cover index page
default_cover_detail: "http://placehold.it/1300x500"

### Social Account

Setup the links to your social pages in the theme's `_config.yml`. Links are in the footer.

```
# Social Accounts
twitter_url:
facebook_url:
behance_url:
googleplus_url:
dribble_url: 
rss_url:
```

## Post Custom Configuration

For each post, you can specify additional information in the [front matter](https://hexo.io/docs/front-matter.html)

### Post's Index Thumbnail

Use `cover_index` to specify an image that will be used for that post on the Home page (also knows as index)

Example:

```
cover_index: /assets/work1.jpg
```

### Post's Detail Thumbnail

Use `cover_detail` to specify an image that will be used for that post on the Detail page for that post.

```
cover_detail: /assets/hero_image.jpg
```
