smilify
=========
`smilify` is a [Liquid](http://www.liquidmarkup.org/) filter to transform text
emoticons into smileys.
It can be easily plugged in to your existing Jekyll powered content to bring
all your text emoticons to life.  
Take a look at my blog: [http://saswatpadhi.github.com/](), powered by `smilify`  
You can also read my post about it: http://saswatpadhi.github.com/blog/2012/06/13/my-first-jekyll-plugin-smilify/.

### Using `smilify` ###
-----------------------
To use smilify in your existing Jekyll powered website,

1. **Copy required files**
  * Copy the content of `plugins` folder to the `_plugins` or `plugins` folder
    as per your configuration.  
    [Learn more about `_plugins` folder here: [https://github.com/mojombo/jekyll/wiki/Plugins]()]
  * Copy the contents of `source/images` to the `images` folder in
    the root folder of your blog source.  
    [Learn more about `source` folder here: [https://github.com/mojombo/jekyll/wiki/Configuration]()]
  * Copy the contents of `source/_include to the `_include` folder.  
    [Learn more about `_include` folder here: [https://github.com/mojombo/jekyll/wiki/Configuration]()]

2. **Choose a smiley theme**
  * `smilify` comes with 3 smiley packs, assembled from various sources.  
    To use a particula smiley pack in your website, you just have to add one line to your `_config.yml`:

    ```ruby
        smileytheme: MSN        # Use the MSN smiley theme
    ```

3. **Apply the filter in your Liquid templates**
  * For `smilify` to detect and _smilify_ your text emoticons, your content must be passed through 
    the `smilify` filter.  
    How and where you apply the filter would depend on thw way you have organised your Liquid template,
    but for most people, changing `_post.html` and `_page.html` in the `_layouts` folder should just work.  
    <br>
    If you have something like `{{ content }}` somewhere in your layout, just pipe it through `smilify`, like:
    `{{ content | smilify }}`

### Custom smiley packs ##
--------------------------
Please refer to [Smiley-Packs](https://github.com/SaswatPadhi/jekyll_smilify/wiki/Smiley-Packs) wiki page.

### LICENSE ###
---------------
Copyright &copy; 2012 Saswat Padhi under MIT License  
[Please Refer included [LICENSE](https://raw.github.com/SaswatPadhi/jekyll_smilify/master/LICENSE)
file for more information]

smiley images are owned by their respective creators.
