# slideshare-slides

An element showing a SlideShare slideset. Embedding a SlideShare presentation gets as easy as
```
<slideshare-slideset slides-id="47323971&doc=2015-150423044157-conversion-gate02">
</slideshare-slideset>
```
...where `id` is the id you get through the WordPress embed code after clicking "Share" below any slideshow on
slideshare.net. 

**Disclaimer:** This piece of software is not developed or supported by SlideShare or LinkedIn. It is developed
independently by the community, however it may use libraries or depend on functionalities provided by SlideShare.

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


## Playing With The Element

If you wish to work on the element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at
`http://localhost:8080/components/slideshare-slides/`.


## Linting The Element

If you wish to lint your element, we recommend that you use
[Polylint](https://github.com/PolymerLabs/polylint) to take into account Polymer 
linting specificities. You can install it via:

    npm install -g polylint

And you can run it via:

	polylint -i seed-element.html

If your element contains errors, they will appear on the console.

Note that it is possible to use `Polylint` with Atom and Sublime with the appropriate package/plugin.

For more options regarding `polylint`, please refer to the 
[documentation](https://github.com/PolymerLabs/polylint#polylint).


## Testing Your Element

Simply navigate to the `/test` directory of your element to run its tests. If
you are using Polyserve: `http://localhost:8080/components/seed-element/test/`

### web-component-tester

The tests are compatible with [web-component-tester](https://github.com/Polymer/web-component-tester).
Install it via:

    npm install -g web-component-tester

Then, you can run your tests on _all_ of your local browsers via:

    wct

#### WCT Tips

`wct -l chrome` will only run tests in chrome.

`wct -p` will keep the browsers alive after test runs (refresh to re-run).

`wct test/some-file.html` will test only the files you specify.
