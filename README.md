# Bloket blog


## How to run 
```docker run --name blog --volume="$PWD:/srv/jekyll" -p 4000:4000 -it jekyll/jekyll jekyll serve```


## Site Configuration

There is a configuration file `_config.yml` in root directory. You should overwrite it to fit to your needs.

## Favicons
- `apple-touch-icon.png` (180x180)
- `favicon-32x32.png` (32x32)
- `favicon-16x16.png` (16x16)
- `mstile-150x150.png` (150x150)
- `android-chrome-192x192.png` (192x192)
- `android-chrome-512x512.png` (512x512)

in `/assets` directory. They're easily created via [Favicon Generator](https://realfavicongenerator.net/).


## Related Articles

Related articles section is based on article tags. For every post that you want to have this section you should define tags.
To include related articles in the bottom of the content you should define `related_posts_section` property in configuration file.
It contains two fields: `max_count` and `min_common_tags`:
- `max_count` represents the maximum number of related articles shown on a single article.
- `min_common_tags` represents the minimum number of common tags for two articles to become related articles.

## Links to social media

To include links to social media in the top right corner of your page you need to define `social` property.
It contains email, GitHub, Twitter and LinkedIn fields. You can leave out any of these if you don't want them to show up on your page.

## Customizing Rain theme

If you want to customize Rain theme you can fork this project and make some changes. If you just want to change the style then you can find Sass files in `_sass/rain` directory.

## Adding your own posts

You can see an example of post structure in `_posts` directory. After you clone this project you should clean the `_posts` directory and add your own posts.

## Build and serve

```
bundle exec jekyll serve
```

Head over to http://127.0.0.1:4000/ to see your page.

## License

Rain is licensed under the MIT license. Check the [LICENSE](LICENSE.md) file for details.

## Author

[Inela Avdic Hukic](https://github.com/inelaah)
