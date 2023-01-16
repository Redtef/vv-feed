# News Feed Eradicator

A browser extension that deletes the main feed on your social media of choice
and replaces with a visual from [Visualize Value](https://visualizevalue.com/) by [@Jackbutcher](https://twitter.com/jackbutcher).

This Extension is also based on the work of [News Feed Eradicator](https://github.com/jordwest/news-feed-eradicator) by [@JordWest](https://github.com/jordwest). Which replaces your news feed by a nice Quote.

[Install Chrome Extension](https://chrome.google.com/webstore/detail/news-feed-eradicator-for/fjcldmjmjhkklehbacihaiopjklihlgg?hl=en)

[Install Firefox Add-on](https://addons.mozilla.org/en-US/firefox/addon/news-feed-eradicator/)

![Screenshot]("https://github.com/Redtef/vv-feed/blob/master/assets/screenshot.png")

## Development

This plugin is built as a WebExtension - a standard for browser plugins currently supported in both Chrome and Firefox.

To build for either browser, clone the repository and then run:

    make dev

If everything is successful, check the `build` folder for the extension contents. You can load the `build` directory into either Chrome or Firefox as an _unpacked_ or _temporary_ extension. See the instructions for [Chrome](https://developer.chrome.com/extensions/getstarted#unpacked) or [Firefox](https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox).

Running `make dev` will watch for changes and recompile, however each time you make changes you'll need to tell the browser to reload the temporary extension.

To build a distributable `.zip` for production, just run:

    make

The extension package can be found in the `dist` folder.
