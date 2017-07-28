Markdown Liquid syntax for Sublime Text 3
=========================================
I use always use [Jekyll][] which uses [Liquid][] for static sites and blogs.

With the additional features of Liquid, Markdown syntax highlighting alone just doesn’t cut it.

Siteleaf have made an excellent [Liquid HTML syntax package][html], but any writing I do is Liquid Markdown.

Here is how you install my “package” via GitHub:

1. Install [Package Control](https://packagecontrol.io/installation)
2. (CTRL+Shift+P|CMD+Shift+P): Add Repository
3. Enter `https://github.com/ndarville/markdown-liquid-syntax`
4. (CTRL+Shift+P|CMD+Shift+P): Install Package
5. Select the package to install
6. Select your new **Markdown Liquid** syntax

Done.

You may have to run Upgrade Package for this, but I honestly have no idea how it works.

As of now, the default associations are:

```yaml
- markdown
- md
- mdown
- txt
```

Currently, the default `<pre>` syntax is `{% highlight lang %}` and `{% endhighlight %}` from Liquid. I have only set up syntax highlighting inside to work with JavaScript and Shell scripts. This is to avoid having a major list of supported programming or markup languages I won’t be using anyway.

You can fork the project to edit the list and just add that repo instead of mine and use that. It’s way easier than demanding I change it in a pull request. The fairly short and simple source code should make it a lot easier for you than starting from scratch. I found the official documentation to be beyond awful; it doesn’t even have bloody pagination.

After all, editors setups are very personal things; I just found the experience of making a ST3 syntax to be an absolute pain, so here’s a template you can use to add and edit to your own liking.

I’ve also included a settings file because, for one, I hate not having line wrap. Second, it sets the file associations so you shouldn’ve have to fiddle with syntax settings yourself. Here is what it looks like:

```json
{
    "extensions": [
        "markdown",
        "mdown",
        "md",
        "txt"
    ],
    "wrap_width": 78
}
```

For more on customizing Sublime Text 3 and your editor and programming experience, check out my [style repo][] with my other configs.


[jekyll]: https://jekyllrb.com
[liquid]: https://shopify.github.io/liquid/
[html]: https://github.com/siteleaf/liquid-syntax-mode
[style]: https://github.com/ndarville/style
