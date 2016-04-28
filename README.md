# jquery-console.js
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
### 5. Invoke the console ###

```html
<script type="text/javascript">
	c.log('Added!');
    c.success('Yes!');
    c.error('Oops!');
    c.warning('Alert!');
</script>
```
## License ##

The plugin is available under the <a href="http://opensource.org/licenses/MIT">MIT license</a>.