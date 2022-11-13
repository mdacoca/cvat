---
title: 'Annotation with brushing tools'
linkTitle: 'Annotation with brushing tools'
weight: 13
description: 'Guide to annotating tasks using  brushing tools.'
---

The brushing tool creates a segmentation mask (further - mask).

Use it, when you need to add a label to an object that has several separated parts, but must be counted as one, for example - a house hiding behind trees or a pillar behind a traffic sign.

You can annotate images manually or upload already annotated images, you can use both: brush and polygon tools on the same image.

See:

- [Brushing tools menu](#brushing-tools-menu)
- [Annotation with brush](#annotation-with-brush)
- [Annotation with polygon-to-mask](#annotation-with-polygon-to-mask)
- [Remove underlying pixels](#remove-underlying-pixels)
- [Import and export](#import-and-export)

## Brushing tools menu

The brushing tool menu appears on the top of the screen after you click **Shape**:

![BT Menu](/images/brushing_tool_menu.png)

It has the following elements:

|Element|Description|
|----|-----|
|![Tick icon](/images/tick_icon.png)| **Save mask** saves the created  mask. The saved mask will appear on the object sidebar|
|![Save mask and continue](/images/brushing_tools_add_label.png)| **Save mask and continue** adds a new mask to the object sidebar, and allows you to draw a new one immediately.|
|![Brush](/images/brushing_tools_icon.png)| **Brush**  applies the mask to the object.|
|![Eraser](/images/brushing_tools_erase.png)|**Eraser** removes part of the mask.|
|![Add poly](/images/brushing_tools_add_poly.png)|**Polygon**  selection tool. Selection will become a mask.|
|![Remove poly](/images/brushing_tools_remove_poly.png)|**Remove polygon selection** substracts part of the polygon selection.|
|![Brush size](/images/brushing_tools_brush_size.png)|**Brush size** in pixels. <br>**Note:** Visible only when **Brush** or **Eraser** are selected.|
|![Brush shape](/images/brushing_tools_brush_shape.png)|**Brush shape** with two options: circle and square. <br>**Note:** Visible only when **Brush** or **Eraser** are selected.|
|![Pixel remove](/images/brushing_tools_pixels.png)|**Remove underlying pixels**. When you are drawing or editing a mask with this tool, <br>pixels on other masks that are located at the same positions as the pixels of the <br>current mask are deleted.|
|![Label](/images/brushing_tools_label_drop.png)|**Label** that will be assigned to the newly created mask||
|![Move](/images/brushing_tools_brush_move.png)|**Move**. Click and hold to move the menu bar to the other place on the screen|



## Annotation with brush

Prerequisites: [Create task](/docs/manual/basics/creating_an_annotation_task/), upload the image, add labels, and open the workspace.

Do the following:

1. From the [controls sidebar](/docs/manual/basics/controls-sidebar/), select **Brush** ![Brush icon](/images/brushing_tools_icon.png).
2. In the **Draw new mask** menu, select label for your mask, and click **Shape**. <br>The **Brush**![Brush](/images/brushing_tools_icon.png) tool will be selected by default.

   ![BT context menu](/images/brushing_tools_context_menu.png)

3. With the brush, draw a mask on the object you want to label. <br>To correct selection, use **Eraser** ![Eraser](/images/brushing_tools_erase.png)

   ![Brushing](/images/brushing_tools.gif)

4. After you applied the mask, on the top menu bar click **Save mask** ![Tick icon](/images/tick_icon.png) to finish the process (or **N** on the keyboard).
5. Added object will appear on the [objects sidebar](/docs/manual/basics/objects-sidebar/).

To add the next label, repeat steps 1 to 5. All added labels will be visible on the image and the  [objects sidebar](/docs/manual/basics/objects-sidebar/).

To save the job  with all added labels, on the top menu click **Save** ![Save](/images/brushing_tools_save.png).



## Annotation with polygon-to-mask

Prerequisites: [Create task](/docs/manual/basics/creating_an_annotation_task/), upload the image, add labels, and open the workspace.

Do the following:

1. From the [controls sidebar](/docs/manual/basics/controls-sidebar/), select **Brush** ![Brush icon](/images/brushing_tools_icon.png).
2. In the **Draw new mask** menu, select label for your mask, and click **Shape**.

   ![BT context menu](/images/brushing_tools_context_menu.png)

3. In the brushing tool menu, select **Polygon** ![Add poly](/images/brushing_tools_add_poly.png).
4. With the **Polygon**![Add poly](/images/brushing_tools_add_poly.png) tool, draw a mask for the object you want to label. <br>To correct selection, use **Remove polygon selection** ![Remove poly](/images/brushing_tools_remove_poly.png).
5. Use **Save mask** ![Tick icon](/images/tick_icon.png) (or **N** on the keyboard) to switch between add/remove polygon tools:

   ![Brushing](/images/brushing_tools_polygon.gif)

6. After you added the polygon selection, on the top menu bar click **Save mask** ![Tick icon](/images/tick_icon.png) to finish the process (or **N** on the keyboard).
7. Click **Save mask** ![Tick icon](/images/tick_icon.png) again (or **N** on the keyboard). Added object will appear on the [objects sidebar](/docs/manual/basics/objects-sidebar/).

To add the next label, repeat steps 1 to 5. All added labels will be visible on the image and the  [objects sidebar](/docs/manual/basics/objects-sidebar/).

To save the job  with all added labels, on the top menu click **Save** ![Save](/images/brushing_tools_save.png).


## Remove underlying pixels

Use **Remove underlying pixels** tool  when you want to add mask and simultaneously delete the pixels of other masks that are located at the same positions. It is highly useful feature to avoid meticulous drawing edge twice between two different objects


![Remove pixel](/images/brushing_tools_pixel_underlying.gif)

## Import and export

For export, see [Export dataset](/docs/manual/advanced/export-import-datasets/)

Import follows the general [import dataset](/docs/manual/advanced/export-import-datasets/) procedure, with the additional option of converting masks to polygons.

>**Note:** This option is available for formats that work with masks only.

To use it, when uploading the dataset, switch the **Convert masks to polygon** toggle to the right:

![Remove pixel](/images/brushing_tools_import.png)







