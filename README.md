# jquery.console.js
A built-in console to be displayed within the HTML view.


Main features: 

* Display logs in your code.
* Separate logs, errors, warnings and success messages.
* Excellent if you are developing cordova apps and want to see console messages.
* Timestamped.
* Customizable height and width.
* Infinite scrolling logs, in little real estate
* carousel layout
* full width and full window support



## Getting started ##

### 1. Get a copy of the plugin ###

You can fork or download the plugin from GitHub


### 2. Load the required files ###


In the page's footer, just before <code>&lt;/body&gt;</code>, include the required JavaScript files.

```html
<script src="libs/js/jquery-1.11.0.min.js"></script>
<script src="dist/js/jquery.console.js"></script>
```

### 3. Create the HTML markup ###

```html
<div id='debug'></div>
```

### 4. Instantiate the console ###

```html
<script type="text/javascript">
	var c=new Console({
            'element':'#debug',
            'width':500,
            'height':100,
            'bg':'#efefef'
        });
</script>
```

Or simply,

```html
<script type="text/javascript">
	var c=new Console();
</script>
```

### 5. Invoke the console ###

```html
<script type="text/javascript">
	c.log('Added!');
    c.success('Yes!');
    c.error('Oops!');
    c.warning('Alert!');
</script>
```

### 6. Options ###

The options available for passing to `Console()`: 

* `element` - The element selector. Default `#debug`
* `width` - Width of the console in `px`. Default `500`
* `height` - Height of the console in `px`. Default `100`
* `bg` - Background color of the console. Default `#efefef`
* `padding` - Padding of the console. Default `5`
* `search_border` - Border of the search input. Default `1px SOLID #fefefe`
* `search_btn_border` - Border of search button. Default `1px SOLID #ffffff`
* `search_bg` - Background color of search input. Default `#f8f8f8`
* `search_btn_bg` - Background color of search button. Default `#fefefe`
* `search_color` - Text color of search input. Default `#555`
* `search_btn_color` - Text color of search button. Default `#888`


## License ##

The plugin is available under the <a href="http://opensource.org/licenses/MIT">MIT license</a>.