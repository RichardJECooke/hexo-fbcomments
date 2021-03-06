# hexo-fbcomments

A simple way to add Facebook comments support to your Hexo posts.

## Usage

1. In your Hexo website folder type `npm install hexo-fbcomments`
2. Put the following code inside your `_config.yml` and set the the appId to the one for your site you've created on Facebook for developers.
``` yml
# Facebook comments - https://github.com/RichardJECooke/hexo-fbcomments/
fbcomments:
  appId: 0 # <---- TODO
  colorscheme: dark # (optional) light/dark
  enabled: true # (optional) true/false
  lang: en_US # (optional)
  order_by: time  # (optional) time/reverse_time/social
  numPosts: 10 # (optional) defaults to 5
```
3. Add ```<%- fbcommentshead() %>``` in your theme's post header (before the body tag) and ```<%- fbcomments(page.permalink) %>``` at the bottom of the post.
4. To style the comments add something like this in your CSS
```css
  section#comments {
    border-color: white;
    border: 1px 1px 1px 1px;
    border-style: solid;
    background: #dde !important;
  }
```

## More
- More information about the facebook comments plugin on the [Official Documentation](https://developers.facebook.com/docs/plugins/comments)
- Created by Sergio Moura.
- Maintained by Richard Cooke.
- License: **MIT**
