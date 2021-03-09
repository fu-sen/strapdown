## Strapdown.js

[Strapdown.js](http://strapdownjs.com/) makes it embarrassingly simple to create elegant Markdown documents. No server-side compilation required. 

For more, please see:

- https://strapdown.js.balloon.net.eu.org/4 - Bootstrap 4 themes
- https://strapdown.js.balloon.net.eu.org/3 - Bootstrap 3 themes
- https://strapdown.js.balloon.net.eu.org/2 - Bootstrap 2 themes

Tip: The original Strapdown.js is a **Bootstrap 2 theme**

___

## Original Project

Oops! This is a forked project. The original README.md can be found here:

[README.original.md](https://github.com/fu-sen/strapdown/blob/main/README.original.md)

See original project if needed:

<https://github.com/arturadib/strapdown>

___

## Version and Branch

I split the branch according to the version of Bootstrap themes

|Themes     |Version|Source branch|
|-----------|:-----:|:-----------:|
|Bootstrap 4| v0.4  | main        |
|Bootstrap 3| v0.3  | bootstrap3  |
|Bootstrap 2| v0.2  | bootstrap2  |

The main changes from the original are:

- Add theme (v0.2 only)
- Add CSS (v0.4 only)
- Change padding-top `60px` to `90px` (Consideration of lux, v0.4 only)
- Updates in `vendor/` (Includes themes)
- Change `nav` class in `strapdown.js`
- Change `viewport` of `strapdown.js`

Bootstrap 3 is effectively this fork. Great job, @bhhaskin !:

- <https://github.com/arturadib/strapdown/pull/51>
- <https://github.com/OCG-labs/strapdown/tree/dev>

___

## Add CSS (v0.4)

Bootstrap 4 has major changes to the CSS specification. I needed to add strapdown.css for this.

The following is considered in Strapdown.js v0.4 (Same as v0.2 and v0.3). This is necessary because it inherits the style of Google Code Prettify:

- `<pre><code>`
- `<code>`

The following is not taken into consideration. You can apply Custom CSS if necessary.

- `<blockquote>` (Changed it to use `class="blockquote"` )

___

## CDN

Now we can apply the CDN using [jsDelivr](https://www.jsdelivr.com/). I have prepared different projects for the CDN:

- <https://github.com/fu-sen/strapdown.js>

___

## Contributor guide

The build in this project inherits the original:

You will need Node.js (>0.6.x) and CoffeeScript to generate the bundles. To bundle/compile the assets, issue in the project directory:

```
$ npm install
$ coffee bundle <version_number>
```

Bug fixes should go in the latest version - no need to bump it. New features or anything that changes the old behavior should go into a bumped version.

___

## License

[MiT License](https://github.com/fu-sen/strapdown/blob/main/LICENSE)

日本語: <https://mit.balloon.net.eu.org/>

Excludes `vendor/` and themes. These are licensed separately.
