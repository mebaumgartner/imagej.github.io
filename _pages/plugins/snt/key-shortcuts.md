---
autogenerated: true
title: SNT › Key Shortcuts
description: test description
---

{% include sntnavbar%}



{% capture text%}
Most SNT features are triggered by keyboard shortcuts. Shortcuts are typically single keystrokes and do not require other modifier keys to be pressed. Most are highlighted in the user interface. E.g., to toggle the *<u>H</u>essian analysis* checkbox, one only needs to press its highlighted letter, i.e., {% include key content='H' %}.
{% endcapture %}
{% include ambox text=text %}

### Interactive Prompt

These shortcuts are always available:

-   {% include key content='Y' %} - Confirms the current temporary path. *Mnemonic: <u>Y</u>es*.

<!-- -->

-   {% include key content='N' %} - Discards the current temporary path. *Mnemonic: <u>N</u>o*.

<!-- -->

-   {% include key content='F' %} - Finishes a path. Note that you can finish a path by pressing {% include key content='Y' %} twice.

<!-- -->

-   {% include key content='C' %} - Cancels a path. Note that you can finish a path by pressing {% include key content='N' %} twice.

<!-- -->

-   {% include key content='Esc' %} - Aborts current operation / Exits current mode

### Tracing

These shortcuts are available when running SNT in *Tracing Mode*:

-   {% include key content='H' %} - Toggles <u>H</u>essian calculation of Path curvatures.

<!-- -->

-   {% include key content='I' %} - Toggles tracing on filtered <u>I</u>mage.

<!-- -->

-   {% include key content='M' %} - Finds the brightest voxel (<u>M</u>aximum) above and below the current x,y position and automatically clicks on it. If multiple maxima exist, their average positioning is used. Note that this feature assumes that neurites are brighter than the background.

<!-- -->

-   {% include key content='S' %} - Toggles cursor <u>S</u>napping: If enabled, the plugin will automatically move the cursor to the brightest voxel within the specified x,y,z snapping window<sup>1</sup>. This facilitates accurate [positioning of path points](/plugins/snt/step-by-step-instructions#accurate-point-placement) and it is described in more detail in this [issue](https://github.com/fiji/Simple_Neurite_Tracer/issues/1).

<!-- -->

-   {% include key content='Alt\|Shift' %}-click - Selects a point along the active path to be used as forking point (See [step-by-step instructions](/plugins/snt/step-by-step-instructions#branching-start-a-path-on-an-existing-path) for more details on joining and branching).

### Navigation and Zoom

These shortcuts are always available:

-   {% include key content='Shift' %} - Synchronizes XY, ZY, and XZ views while moving the cursor when not using cursor snapping.

<!-- -->

-   {% include key content='+' %} - Zooms in (Simultaneously on all views) (IJ default).

<!-- -->

-   {% include key content='-' %} - Zooms out (Simultaneously on all views) (IJ default).

<!-- -->

-   {% include key content='4' %} - Displays tracing view(s) at original scale (IJ default).

<!-- -->

-   {% include key content='5' %} - Displays tracing view(s) at 100% (IJ default).

<!-- -->

-   {% include key content='Spacebar' %} - Activates the Pan (Hand) tool (IJ default).

<!-- -->

-   {% include key content='&gt;' %} / {% include key content='&lt;' %} - Previous/Next Z-slice, or Previous/Next channel, depending on the *Reverse CZT oder of "&gt;" and "&lt;"* choice set in IJ's {% include bc path='Edit|Options|Misc..'%} prompt (IJ default).

<!-- -->

-   {% include key content='enter' %} - Shuttles the window focus between the tracing image and the SNT window.

### Path Handling

These shortcuts are always available:

-   {% include key content='1' %} - Toggles the first visibility filter: Whether all traced paths should be displayed or just selected ones

<!-- -->

-   {% include key content='2' %} - Toggles the second visibility filter: Whether all nodes should be displayed across the Z-stack or just those in nearby Z-slices

<!-- -->

-   {% include key content='3' %} - Toggles the third visibility filter: Whether paths from all channels/frames should be displayed or just those in the active channel/frame

<!-- -->

-   {% include key content='G' %} - Selects the nearest path to the mouse cursor. Holding {% include key content='Shift\|G' %} adds the path nearest to the mouse cursor to the current list of selected paths. *Mnemonic: <u>G</u>roup paths around cursor.* Note that Paths can only be edited one at a time, and thus {% include key content='Shift\|G' %} is disabled in *Edit Mode*.

### Path Editing

These shortcuts become available in *Edit Mode*, activated through the contextual menu (displayed when right-clicking on a tracing canvas):

-   {% include key content='D' %} or {% include key content='Backspace' %} - <u>D</u>eletes the active node.
-   {% include key content='I' %} or {% include key content='Insert' %} - <u>I</u>nserts a new node at cursor position.
-   {% include key content='M' %} - <u>M</u>oves active node to cursor position.
-   {% include key content='B' %} - <u>B</u>rings active node to current Z-plane.

### Reconstruction Viewer

-   {% include key content='left' %} {% include key content='right' %} {% include key content='up' %} {% include key content='down' %} - Rotate (with mouse: Left-click & drag)
-   {% include key content='shift' %} + {% include key content='left' %} {% include key content='right' %} {% include key content='up' %} {% include key content='down' %} - Pan (with mouse: Right-click & drag)
-   {% include key content='+' %} {% include key content='-' %} - Zoom (with mouse: Scroll wheel)
-   {% include key content='A' %} - Toggle <u>A</u>xes
-   {% include key content='C' %} - Toggle <u>C</u>amera Mode
-   {% include key content='D' %} - Toggle <u>D</u>ark Mode
-   {% include key content='F' %} - <u>F</u>it View to Visible Objects
-   {% include key content='L' %} - <u>L</u>og Scene Details to Console
-   {% include key content='R' %} - <u>R</u>eset View
-   {% include key content='S' %} - Save <u>S</u>creenshot
-   {% include key content='H' %} - <u>H</u>elp (as Notification) ({% include key content='F1' %} shows Help on a dedicated window)

### SciView

-   Drag - Move around
-   {% include key content='Shift\|' %}+Drag - Rotate around selected node
-   Single-click - Select node
-   Double-click - Centers clicked node
-   {% include key content='Shift\|' %}+Scroll - Zoom
-   {% include key content='W' %} {% include key content='A' %} {% include key content='S' %} {% include key content='D' %} - Move around (hold {% include key content='Shift' %} for slow movement)

See [SciView](/plugins/sciview)'s {% include bc path='Help| '%}menu for a full list of shortcuts.

### Legacy 3D Viewer

All shortcuts that are not specific to tracing canvases (XY, ZY and XZ views) *should* be recognized by the [Legacy 3D viewer](/plugins/snt/step-by-step-instructions#legacy-3d-viewer). In addition the following are also implemented:

-   {% include key content='H' %} - Selects the <u>H</u>and (rotation) tool.
-   {% include key content='W' %} - Selects the <u>W</u>and (selection) tool.
-   {% include key content='Esc' %} - Shuttles between the Hand and Wand tool after both have been selected at least once.

### Other

There are other key and mouse combinations used in e.g., [Sholl Analysis (by Focal Point)](/plugins/snt/analysis#sholl-analysis), and [Branching and Joining Paths](/plugins/snt/step-by-step-instructions#branching-start-a-path-on-an-existing-path), that are listed in the contextual menu, displayed when righ-clicking a tracing canvas.


{% capture tip%}
SNT was designed so that its shortcuts do not collide with those of ImageJ. SNT hotkeys do not require holding down {% include key content='Control' %} ({% include key content='Cmd' %} on MacOS). When such a modifier key is pressed, the hotkey will no longer be intercepted by SNT. E.g., During a tracing session pressing {% include key content='S' %} will toggle cursor snapping while Pressing {% include key content='Control\|S' %} ({% include key content='Cmd\|S' %}on MacOS) will allow you to save the traced image using IJ"s built-in command {% include bc path='File|Save'%}.
{% endcapture %}
{% include tip tip=tip %}

{% include sntnavbar%}