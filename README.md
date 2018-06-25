# vdl-custom-extensions
Library of prototype VDL custom extensions for FICO Xpress Insight

## Notice

These VDL Extensions are named with the <code>vdlx-</code> prefix. 
This means that they are written by the Xpress Insight VDL team and are earmarked for possible inclusion in a future version of the software.
It is recommended that you keep up to date with any changes to this software. 

If any of these extensions are included in the product then they will be deprecated here and will appear in Xpress Insight with the normal <code>vdl-</code> prefix.

You are welcome to use these extensions in your VDL apps and to learn from the source code in creating your own extensions. When developing custom extensions please use another namespace so that there is no confusion between your own custom extensions and the official ones. 

#### Usage
Zip up the whole directory, minus this README and the LICENSE files, then upload the zip archive to your instance of Xpress Insight 4.x.

After loading a new App will be available named: 'VDL Extensions Demo'.

#### Extensions Usage

The <code>includes</code> contains the custom extension source. Use <code><vdl-include src="vdlx-extension-name.vdl"/></code> where <code>extension-name</code> is one of these custom extensions to include in your view. The relevant tag will then be usable within your app. 

#### Current Extensions

* <code>vdlx-sidebar</code> - the main sidebar extension
* <code>vdlx-toolbar</code> - a simple toolbar, usually top of view [discussion](./client_resources/includes/vdlx-toolbar.md)
* <code>vdlx-dropdown-button</code> - a dropdown menu
* <code>vdlx-tabs</code> - tabs or pills for inner view navigation
* <code>vdlx-modal</code> - a modal dialog wrapper that can contain custom VDL [discussion](./client_resources/includes/vdlx-modal.md)

There are other component demos within this repository that were simpler to create with exisitng VDL and HTML rather than creating a custom extension. 

#### Get involved

We will be accepting pull requests and feature requests and defect fixes so please contact us if you have Xpress Insight app requirements that may be enhanced with custom extensions.

Joc O'Connor - 
VDL Technical Lead for FICO Xpress Insight

The code in this repository is covered by the Apache 2 Licence.