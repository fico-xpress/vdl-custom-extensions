# VDL Custom Extension
## vdlx-modal
#### A VDL Extension that provides modal dialog functionality

This extension allows the wrapping of VDL content within the `<vdlx-modal>` tag in order to provide that content in a modal dialog when triggered.

#### Usage
```
<script>
    function showDemo() {
        $('#demo-modal').trigger('showModal');
    }
</script>
<a id="demo-btn" vdl-event="click: showDemo" class="btn">Show</a>
<vdlx-modal id="demo-modal" title="Settings panel">
    <h3>Settings controls here</h3>
</vdlx-modal>
```
This example displays a button that, when clicked, launches a modal dialog with the title taken from the `title` attribute.

![vdlx-modal](../gfx/vdlx-modal1.png) 