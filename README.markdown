Markdown Liquid syntax for Sublime Text 3
=========================================

1. Install [Package Control](https://packagecontrol.io/installation)
2. (CTRL+Shift+P|CMD+Shift+P): Add Repository
3. Enter `https://github.com/ndarville/markdown-liquid-syntax`
4. (CTRL+Shift+P|CMD+Shift+P): Install Package
5. Select the package to install
6. Select your new **Markdown Liquid** syntax

Done.

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
