---
tags: runtime-traditionalweb; 
summary: Responsive Table displays information in a logical and organized way that is easy to scan and read.
---

# Responsive Table

<div class="info" markdown="1">

We’ve been working on this article. Please let us know how useful this new version is by voting.

</div>

You can use the Responsive Table UI Pattern to display information in a logical and organized way. The Responsive Table UI pattern allows interaction, such as sorting, so that users can customize how they view information.

**How to use the Responsive Table UI Pattern**

The Responsive Table UI Pattern usually displays dynamic information. In most cases, prior to using this pattern, you will need [to retrieve or update the Data](../../../../../develop/data/intro.md) that contains the information you want to display onscreen. You do this by using an [Action](../../../../../develop/logic/action-web.md).

The following example demonstrates how you can display the registered users on your platform.

1. In Service Studio, in the Toolbox, search for `Responsive Table`.

    The Responsive Table widget is displayed.

    ![](<images/responsivetable-8-ss.png>)

    If the UI widget does not display, it may be because you used a ready-made app, which deletes unused widgets from the module. To make additional widgets available in your app:

    a. Go to **Module > Manage dependencies**.

    b. Search for and select the relevant Producer, for example OutSystemsUI. Ensure Show All is selected. 

    c. On the Public elements for the selected Producer displayed on the right, ensure Show All is selected.
    
    d. Search for and select the element you want to add, and click **Apply**. 
    
    e. In Service Studio, in the Toolbox, search for the widget again.

1. From the Toolbox, drag the Responsive Table widget into the Main Content area of your application's screen.

    ![](<images/responsivetable-1-ss.png>)

1. Select the **Data** tab, and from the Entities tree, navigate to the **User** entity and drag it into the Responsive Table placeholder.

    ![](<images/responsivetable-10-ss.png>)

1. To reopen your screen, select the **Interface** tab, and double-click on your screen.

1. On the **Properties** tab, set the **ResponseBehavior** property. In this example, the property is set so the table header stays fixed and the user can scroll through the rows.

    ![](<images/responsivetable-6-ss.png>)

After following these steps and publishing the module, you can test the pattern in your app.

## Properties

| Property |  Description |
|---|---|
| ResponsiveBehavior (ResponsiveTableRecords Identifier): Mandatory | Define how the table behaves when the user interacts with it. The predefined values are:<p><ul><li>ExpandableRows</li><li>ScrollableRows (default)</li></ul></p> <p>Examples <ul><li>_Entities.RepsonsiveTableRecords.ScrollableRows_ - The table header stays fixed and the user can scroll through the rows in the table. </li><li>_Entities.RepsonsiveTableRecords.ExpandableRows_ - The table header stays fixed and the user can expand each row to view any extra information. </li></ul></p> |
