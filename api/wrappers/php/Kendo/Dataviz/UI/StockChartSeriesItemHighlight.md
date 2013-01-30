---
title: StockChartSeriesItemHighlight
slug: php-dataviz-ui-stockchartseriesitemhighlight
tags: api, php
publish: true
---

# \Kendo\Dataviz\UI\StockChartSeriesItemHighlight

A PHP class representing the highlight setting of StockChartSeriesItem.


## Methods

### border

The border of highlighted points. The color is computed automatically from the base point color.

#### Returns
`\Kendo\Dataviz\UI\StockChartSeriesItemHighlight`

#### Parameters

##### $value `\Kendo\Dataviz\UI\StockChartSeriesItemHighlightBorder|array`


#### Example - using [\Kendo\Dataviz\UI\StockChartSeriesItemHighlightBorder](/api/wrappers/php/kendo/dataviz/ui/stockchartseriesitemhighlightborder)

    $highlight = new \Kendo\Dataviz\UI\StockChartSeriesItemHighlight();
    $border = new \Kendo\Dataviz\UI\StockChartSeriesItemHighlightBorder();
    $color = 'value';
    $border->color($color);
    $highlight->border($border);

#### Example - using array

    $highlight = new \Kendo\Dataviz\UI\StockChartSeriesItemHighlight();
    $color = 'value';
    $highlight->border(array('color' => $color));

### color
The highlight color.** Available only for pie series **

#### Returns
`\Kendo\Dataviz\UI\StockChartSeriesItemHighlight`

#### Parameters

##### $value `string`



#### Example 
    $highlight = new \Kendo\Dataviz\UI\StockChartSeriesItemHighlight();
    $highlight->color('value');

### line

Line options for highlighted points. The color is computed automatically from the base point color.** Available only for candlestick series **

#### Returns
`\Kendo\Dataviz\UI\StockChartSeriesItemHighlight`

#### Parameters

##### $value `\Kendo\Dataviz\UI\StockChartSeriesItemHighlightLine|array`


#### Example - using [\Kendo\Dataviz\UI\StockChartSeriesItemHighlightLine](/api/wrappers/php/kendo/dataviz/ui/stockchartseriesitemhighlightline)

    $highlight = new \Kendo\Dataviz\UI\StockChartSeriesItemHighlight();
    $line = new \Kendo\Dataviz\UI\StockChartSeriesItemHighlightLine();
    $color = 'value';
    $line->color($color);
    $highlight->line($line);

#### Example - using array

    $highlight = new \Kendo\Dataviz\UI\StockChartSeriesItemHighlight();
    $color = 'value';
    $highlight->line(array('color' => $color));

### opacity
The opacity of the highlighted points.

#### Returns
`\Kendo\Dataviz\UI\StockChartSeriesItemHighlight`

#### Parameters

##### $value `float`



#### Example 
    $highlight = new \Kendo\Dataviz\UI\StockChartSeriesItemHighlight();
    $highlight->opacity(1);
