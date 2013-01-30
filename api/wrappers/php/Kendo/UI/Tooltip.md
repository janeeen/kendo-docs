---
title: Tooltip
slug: php-ui-tooltip
tags: api, php
publish: true
---

# \Kendo\UI\Tooltip

A PHP class representing Kendo [Tooltip](/api/web/tooltip).


## Configuration

To use Tooltip in a PHP page instantiate a new instance, configure it via the available
configuration [methods](#methods) and output it by `echo`-ing the result of the `render` method.

### Using Kendo Tooltip

    <?php
    // Create a new instance of Tooltip and specify its id
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');

    // Configure it
    $tooltip->autoHide(true)

    // Output it

    echo $tooltip->render();
    ?>


## Methods

### animation

A collection of {Animation} objects, used to change default animations. A value of false
will disable all animations in the widget.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `\Kendo\UI\TooltipAnimation|array`


#### Example - using [\Kendo\UI\TooltipAnimation](/api/wrappers/php/kendo/ui/tooltipanimation)

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $animation = new \Kendo\UI\TooltipAnimation();
    $close = new \Kendo\UI\TooltipAnimationClose();
    $animation->close($close);
    $tooltip->animation($animation);

#### Example - using array

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $close = new \Kendo\UI\TooltipAnimationClose();
    $tooltip->animation(array('close' => $close));

### autoHide
Specifies if the tooltip will be hidden when mouse leaves the target element. If set to false a close button will be shown within tooltip.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `boolean`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->autoHide(true);

### callout
Specifies if the tooltip callout will be displayed.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `boolean`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->callout(true);

### content

The text or a function which result will be shown within the tooltip.
By default the tooltip will display the target element title attribute content.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction|\Kendo\UI\TooltipContent|array`




#### Example  - using string
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->content('value');

#### Example  - using \Kendo\JavaScriptFunction
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->content(new \Kendo\JavaScriptFunction('function() { }'));


#### Example - using [\Kendo\UI\TooltipContent](/api/wrappers/php/kendo/ui/tooltipcontent)

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $content = new \Kendo\UI\TooltipContent();
    $url = 'value';
    $content->url($url);
    $tooltip->content($content);

#### Example - using array

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $url = 'value';
    $tooltip->content(array('url' => $url));

### contentLoad
Triggered when an AJAX request for content completes.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->contentLoad('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onContentLoad(e) {
            // handle the contentLoad event.
        }
    </script>
    <?php
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->contentLoad('onContentLoad');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->contentLoad(new \Kendo\JavaScriptFunction('function(e) { }'));

### error
Triggered when an AJAX request for content fails.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->error('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onError(e) {
            // handle the error event.
        }
    </script>
    <?php
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->error('onError');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->error(new \Kendo\JavaScriptFunction('function(e) { }'));

### filter
Specifies a selector for elements, within the container, for which the tooltip will be displayed.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `string`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->filter('value');

### height
The height (in pixels) of the tooltip.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `float`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->height(1);

### hide
Triggered when a Tooltip is hidden

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->hide('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onHide(e) {
            // handle the hide event.
        }
    </script>
    <?php
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->hide('onHide');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->hide(new \Kendo\JavaScriptFunction('function(e) { }'));

### iframe
Explicitly states whether content iframe should be created.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `boolean`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->iframe(true);

### position
The position relative to the target element, at which the tooltip will be shown. Predefined values are "bottom", "top", "left", "right", "center".

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `string`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->position('value');

### show
Triggered when a Tooltip is shown.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->show('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onShow(e) {
            // handle the show event.
        }
    </script>
    <?php
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->show('onShow');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->show(new \Kendo\JavaScriptFunction('function(e) { }'));

### showAfter
Specify the delay in milliseconds before the tooltip is shown. This option is ignored if showOn is set to "click" or "focus".

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `float`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->showAfter(1);

### showOn
The event on which the tooltip will be shown. Predefined values are "mouseenter", "click" and "focus".

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `string`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->showOn('value');

### width
The width (in pixels) of the tooltip.

#### Returns
`\Kendo\UI\Tooltip`

#### Parameters

##### $value `float`



#### Example 
    $tooltip = new \Kendo\UI\Tooltip('Tooltip');
    $tooltip->width(1);
