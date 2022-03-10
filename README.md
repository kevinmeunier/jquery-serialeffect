### jquery.serialeffect - An innovative plugin based on jQuery to animate letters on scroll.

## About jQuery serialeffect
jQuery serialeffect has been published on GitHub for educational purpose, it has to be considered as a prototype. Although many optimizations have been developed to improve performance (debounce event, requestAnimationFrame, check FPS, etc.), a lagging effect can appears depending the CPU/GPU. When the FPS are too low, jQuery serialeffect will automatically switch to words animation instead of letters.


## Example
For [documentation](http://jquery.eisbehr.de/lazy/#parameter), [examples](http://jquery.eisbehr.de/lazy/#examples) and other information take a look on the [project page](http://jquery.eisbehr.de/lazy/).


## Compatibility & Performance
jQuery serialeffect is highly performance-consuming if using on the whole page, in order to maintain decent performance, either limit the content on your page, or specify manually a few elements. **The animation effect is disabled on all mobile devices due to poor rendering management with the touch event.**

**Tested in:** IE, Edge, Chrome, Firefox, and Safari.


## Self-Hosted
[Download](https://github.com/kevinmeunier/jquery.serialeffect/archive/master.zip) and save one of two available files to include Lazy to your page, either the [development](http://raw.githubusercontent.com/kevinmeunier/jquery.serialeffect/master/jquery.serialeffect.js) or the [minified](http://raw.githubusercontent.com/kevinmeunier/jquery.serialeffect/master/jquery.serialeffect.min.js) version.
```HTML
<script type="text/javascript" src="jquery.serialeffect.min.js"></script>
```

Make sure [jQuery](http://jquery.com) is properly loaded before calling jQuery serialeffect. 


## Basic Usage
The basic usage of serialeffect is pretty easy, just start using jQuery serialeffect by calling it after page load. You don't have to specify your elements exactly, jQuery serialeffect will find them autonomously based on 'elementsTags' settings ('div, p, li, h1, img, span, a, g' by default).
```JS
$(function($) {
    $(".js-serialeffect").serialeffect();
});
```


## Advanced Usage
To do

## Configuration Parameters
The following configurations is available by default:

Name               | Type       | Default                             | Description
------------------ | ---------- | ----------------------------------- | -----------
autoDetection      | *boolean*  | *true*                              | Find all elligible elements based on *elementsTags* 
sectionsSelector   | *string*   | *'section'*                         | Store elligible elements by sections (in viewport detection)
elementsClass      | *string*   | *js-serialeffect*                   | Add extra elements in the HTML
ignoreClass        | *string*   | *js-serialeffect-ignore*            | Ignore manully any elements from the *elementsTags* 
elementsTags       | *string*   | *'div, p, li, h1, img, span, a, g'* | Elligble elements when *autoDetection* is set to true
maxGap             | *integer*  | *200*                               | Max distance between the original position and the animated position
callback           | *boolean*  | *false*                             | Function called on scroll (after event deboucing)


## Bugs / Feature request
Please [report](http://github.com/kevinmeunier/jquery.serialeffect/issues) bugs and feel free to [ask](http://github.com/kevinmeunier/jquery.serialeffect/issues) for new features directly on GitHub.


## License
jQuery serialeffect is licensed under [MIT](http://www.opensource.org/licenses/mit-license.php) license.
