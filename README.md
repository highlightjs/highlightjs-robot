`highlight.js` syntax definition for Robot Framework.

For more about highlight.js, see https://highlightjs.org/

For more about Robot Framework, see https://robotframework.org/

### Usage

Simply include the `highlight.js` script package in your webpage or node app, load up this module and apply it to `hljs`.

If you're not using a build system and just want to embed this in your webpage:

```html
<script type="text/javascript" src="/path/to/highlight.pack.js"></script>
<script type="text/javascript" src="/path/to/highlightjs-robot/robot.js"></script>
<script type="text/javascript">
    hljs.registerLanguage('robot', window.hljsDefineRobot);
    hljs.highlightAll();
</script>
```

If you're using webpack / rollup / browserify / node:

```javascript
var hljs = require('highlightjs');
var hljsDefineRobot = require('highlightjs-robot');

hljsDefineRobot(hljs);
hljs.highlightAll();
```

While Robot Framework supports [multiple formats](http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#supported-file-formats), currently only space sparated format is supported.

### About the author

Find me at https://spage.fi
