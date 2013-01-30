---
title: PanelBar
slug: php-ui-panelbar
tags: api, php
publish: true
---

# \Kendo\UI\PanelBar

A PHP class representing Kendo [PanelBar](/api/web/panelbar).


## Configuration

To use PanelBar in a PHP page instantiate a new instance, configure it via the available
configuration [methods](#methods) and output it by `echo`-ing the result of the `render` method.

### Using Kendo PanelBar

    <?php
    // Create a new instance of PanelBar and specify its id
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');

    // Configure it
    $panelBar->animation(true)

    // Output it

    echo $panelBar->render();
    ?>


## Methods

### activate
Triggered when an item of a PanelBar is activated.

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->activate('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onActivate(e) {
            // handle the activate event.
        }
    </script>
    <?php
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->activate('onActivate');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->activate(new \Kendo\JavaScriptFunction('function(e) { }'));

### animation

A collection of visual animations used when PanelBar items are exapnd or collapsed through
user interactions. Setting this option to false will disable all animations.

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value `boolean|\Kendo\UI\PanelBarAnimation|array`




#### Example  - using boolean
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->animation(true);


#### Example - using [\Kendo\UI\PanelBarAnimation](/api/wrappers/php/kendo/ui/panelbaranimation)

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $animation = new \Kendo\UI\PanelBarAnimation();
    $collapse = new \Kendo\UI\PanelBarAnimationCollapse();
    $animation->collapse($collapse);
    $panelBar->animation($animation);

#### Example - using array

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $collapse = new \Kendo\UI\PanelBarAnimationCollapse();
    $panelBar->animation(array('collapse' => $collapse));

### collapse
Triggered when an item of a PanelBar is collapsed.

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->collapse('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onCollapse(e) {
            // handle the collapse event.
        }
    </script>
    <?php
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->collapse('onCollapse');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->collapse(new \Kendo\JavaScriptFunction('function(e) { }'));

### contentLoad
Fires when content is fetched from an AJAX request.

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->contentLoad('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onContentLoad(e) {
            // handle the contentLoad event.
        }
    </script>
    <?php
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->contentLoad('onContentLoad');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->contentLoad(new \Kendo\JavaScriptFunction('function(e) { }'));

### error
Fires when AJAX request results in an error.

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->error('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onError(e) {
            // handle the error event.
        }
    </script>
    <?php
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->error('onError');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->error(new \Kendo\JavaScriptFunction('function(e) { }'));

### expand
Triggered when an item of a PanelBar is expanded.

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->expand('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onExpand(e) {
            // handle the expand event.
        }
    </script>
    <?php
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->expand('onExpand');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->expand(new \Kendo\JavaScriptFunction('function(e) { }'));

### expandMode
Specifies how the PanelBar items are displayed when opened and closed. The following values
are available:

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value `string`



#### Example 
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->expandMode('value');

### addItem

Adds one or more PanelBarItem to the PanelBar.

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value[, $value2, ...] `\Kendo\UI\PanelBarItem|array`

#### Example - using \Kendo\UI\PanelBarItem

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $item = new \Kendo\UI\PanelBarItem();
    $contentUrl = 'value';
    $item->contentUrl($contentUrl);
    $panelBar->addItem($item);

#### Example - using array

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $contentUrl = 'value';
    $panelBar->addItem(array('contentUrl' => $contentUrl));

#### Example - adding more than one PanelBarItem

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $first  = new \Kendo\UI\PanelBarItem();
    $second = new \Kendo\UI\PanelBarItem();
    $panelBar->addItem($first, $second);

### select
Triggered when an item of a PanelBar is selected.

#### Returns
`\Kendo\UI\PanelBar`

#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`

#### Example - using string which defines a JavaScript function

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->select('function(e) { }');

#### Example - using string which defines a JavaScript name
    <script>
        function onSelect(e) {
            // handle the select event.
        }
    </script>
    <?php
    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->select('onSelect');
    ?>

#### Example - using [\Kendo\JavaScriptFunction](/api/wrappers/php/kendo/javascriptfunction)

    $panelBar = new \Kendo\UI\PanelBar('PanelBar');
    $panelBar->select(new \Kendo\JavaScriptFunction('function(e) { }'));
