## GitHub Buttons

Basically, a copy-pasta, standalone, Javascript version of [mdo/github-buttons](https://github.com/mdo/github-buttons). The reason for this library is that @mdo's version doesn't work with SSL and using iframes is just silly.

Also, GitHub, you suck for not supporting this yourself.

### Installation

```bash
bower install github-buttons
component install jonathanong/github-buttons
```

### API

Place the buttons wherever on the page. They should have `class="github-btn"`. You may want to have a `class="hide"` as well. You should handle the loading states yourself.

All options as shown on [mdo/github-buttons](https://github.com/mdo/github-buttons) are available through `data-*` attributes. View the demo for basically every possible variation of buttons.

```html
<span class="github-btn hide" data-user="jonathanong" data-repo="github-buttons" data-type="watch" data-count="1"></span>

<script src="github-buttons.js"></script>
```

Note that the script should be loaded after all button definitions.

#### githubButtons(el)

You can load a single button yourself if you'd like. Use this if you load the script before any button definitions.

```js
githubButtons(document.querySelector('.github-btn'))
```

#### githubButtons.all()

Loads all buttons on the page. This is run on script load automatically.

### License

Whatever. WTFPL. It's not really mine.