# VDL Custom Extension
## vdlx-tabs
#### Horizontal pill tabs custom extension. 

A user selecting a pill triggers the `tabChange` event. The `vdl-event` attribute can listen for this event and call the handler when it arrives.

```html
<vdlx-tabs vdl-event="tabChange: horizTabChange">
    <li><a href="#">Home</a></li>
    <li><a href="#">Profile</a></li>
    <li><a href="#">Messages</a></li>
</vdlx-tabs>
```

A small amount of code will enable the developer to create switchable panels.
The event handler should simply set a VDL observable variable.

_Observable means that the value is being watched and will trigger updates when it changes._

This code snippet would perform that function.
```html
<script>
    var horizTab = VDL.createVariable('Home');

    function horizTabChange(vm, evt, tab) {
        horizTab(tab);
    }
</script>
```
Then some VDL code to reveal content based on the value of this `Observable`

```html
<div class="panel" vdl-if="=horizTab() === 'Home'">
    <!-- Home content -->
</div>
<div class="panel" vdl-if="=horizTab() === 'Scripts'">
    <!-- Scripts content -->
</div>
<div class="panel" vdl-if="=horizTab() === 'Child panels'">
    <!-- Child panels content -->
</div>
```

The `vdlx-tabs` extension uses session storage to remember which tab was selected when returning to the view.

![vdlx-tabs](../gfx/vdlx-tabs1.png)