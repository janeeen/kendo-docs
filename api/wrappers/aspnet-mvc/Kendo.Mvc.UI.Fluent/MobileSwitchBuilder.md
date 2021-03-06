---
title:MobileSwitchBuilder
slug:aspnetmvc-kendo.mvc.ui.fluent.mobileswitchbuilder
publish:true
---

# Kendo.Mvc.UI.Fluent.MobileSwitchBuilder
Defines the fluent API for configuring the Kendo MobileSwitch for ASP.NET MVC.



## Methods

### Checked(`System.Boolean`)
The checked state of the widget.


#### Parameters

##### value `System.Boolean`
The value that configures the checked.





### OffLabel(`System.String`)
The OFF label.


#### Parameters

##### value `System.String`
The value that configures the offlabel.





### OnLabel(`System.String`)
The ON label.


#### Parameters

##### value `System.String`
The value that configures the onlabel.





### Events(`System.Action<Kendo.Mvc.UI.Fluent.MobileSwitchEventBuilder>`)
Configures the client-side events.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.MobileSwitchEventBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/MobileSwitchEventBuilder)>
The client events action.




#### Example (ASPX)
    <%= Html.Kendo().MobileSwitch()
    .Name("MobileSwitch")
    .Events(events => events
        .Change("onChange")
    )
    %>



