# github-markdown-css

### GitHub Markdown Flavoured CSS

Less than 200 lines of CSS replicate the GitHub Markdown style. A fork from [sindresorhus/github-markdown-css](https://github.com/sindresorhus/github-markdown-css/), shortened so that the CSS file is smaller but still supports the same features (shortened from 1087 lines to 187 lines). Useful for people who want faster CSS rendering speed.

### Online Demo
Click [here](https://kiwirafe.neocities.org/example) to see the online demo.



## Usage
Download the [github.css](github.css) file and add a `markdown-body` class to the container of the rendered Markdown. 

For example:

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/github.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
    <script>hljs.highlightAll();</script>

    <link rel="stylesheet" href="github.css">
</head>

<body>
    <div class="markdown-body">
        Rendered Markdown here.
    </div>
</body>
</html>
```

### Extra Notes 
1. Include highlight.js before the CSS file if Syntax Highlighting is needed.
2. Inline code should be in `<code>` tags when converted to HTML.
3. Code blocks should be in `<pre><code>` tags when converted to HTML.
