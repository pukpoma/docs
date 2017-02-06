---
title: "Retrieve a list of objects"
category: "howto40"
space: "Mendix 4 How-to's"
---
## Description

This section describes how to retrieve an object or a list of objects in a microflow. The related reference guide article can be found [here](https://world.mendix.com/pages/releaseview.action?pageId=11437399).

## Instructions

![](attachments/819203/917932.png) **Open the microflow, or if necessary create a new one. If you do not know how to add documents to your project, please refer to [this](https://world.mendix.com/display/howto25/Add+documents+to+a+module) article.**

![](attachments/819203/917932.png) **Add a 'Retrieve' activity to the microflow, and double-click on it. If you do not know how to add activities to a microflow please refer to [this](https://world.mendix.com/display/howto25/Add+an+activity+to+a+microflow) article.**

![](attachments/2621588/2752869.png)

The microflow in the screenshot has an 'Order' object passed to it as parameter.

![](attachments/819203/917932.png) **If you choose 'Association' as retrieve type, the activity will retrieve objects by following the specified association. You can select this association by pressing the 'Select' button next to 'Association' and then choose the right association in the menu that pops up. In the case of a reference, the 'Retrieve' activity will return an object, whereas in the case of a reference set it will return a list of objects.**

![](attachments/2621588/2752870.png)

The 'Order' object passed to the microflow makes it possible to retrieve 'Pizza' objects through the 'Order_Pizza' association. Since this is a reference set, the 'Retrieve' activity will return a list of 'Pizza' objects.

![](attachments/819203/917932.png) **If you choose 'From database' as retrieve type, you will need to specify the entity of which you want to retrieve objects, and then provide an XPath expression to constrain the objects which are retrieved.**

![](attachments/2621588/2752867.png)

If you do not provide an XPath expression, the 'Retrieve' activity will return a list of all the objects of the chosen entity.

![](attachments/819203/917932.png) **In the 'Sorting' area of the menu, you can specify attributes you want to sort the list on and then use the drop-down menu to set the sorting to ascending or descending.**

![](attachments/2621588/2752868.png)

You can add new attributes to sort on by pressing the 'New' button.

![](attachments/819203/917932.png) **When you choose the 'From database' option, you can choose to have the 'Retrieve' activity only return the first object, rather than a list of objects by putting a check mark next to 'First object only'.**

![](attachments/2621588/2752857.png)

This can be used if you want it to return a specific object you need for the microflow, rather than a list. However be aware that your XPath expression will need to return the one needed object, or the sorting needs to ensure that the object is the first object on the list for this to work.

![](attachments/819203/917932.png) **For both retrieve methods, you can alter the 'Output variable' to change the variable name which will be used to the returned object or object list in the microflow.**

[![](attachments/819203/917564.png)](Retrieve+a+list+of+objects)[(Back to Top)](Retrieve+a+list+of+objects)