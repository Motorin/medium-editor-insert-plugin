# jQuery insert plugin for MediumEditor

**ATTENTION! This branch is a development branch for version 1.0. If you're looking for a usable version of the plugin, please go to master branch, where you'll find version 0.***

[![Build Status](https://travis-ci.org/orthes/medium-editor-insert-plugin.png?branch=1.0)](https://travis-ci.org/orthes/medium-editor-insert-plugin)
[![Dependency Status](http://www.versioneye.com/user/projects/545a6ed837be08a20d000005/badge.svg?style=flat)](http://www.versioneye.com/user/projects/545a6ed837be08a20d000005)
[![Dependency Status](http://www.versioneye.com/user/projects/545a6f0b37be081d6900002d/badge.svg?style=flat)](http://www.versioneye.com/user/projects/545a6f0b37be081d6900002d)
[![Codacy Badge](https://www.codacy.com/project/badge/1f8565ed2e554e4fa952ec4da6a2080b)](https://www.codacy.com/public/orthes/mediumeditorinsertplugin)

This plugin expands capabilities of [MediumEditor](https://github.com/orthes/medium-editor-insert-plugin/wiki/github.com/daviferreira/medium-editor) (a clone of medium.com WYSIWYG editor) and it enables users to insert into the editor various types of content (depending on available addons).

Current available addons:

- **images**
- **embeds** (either through oEmbed proxy, such as [Iframely](https://iframely.com/), or pre-defined parsers such as - Youtube, Vimeo, Twitter, Facebook, Instagram)


## Screenshots

![jQuery insert plugin for MediumEditor - #1 screenshot](http://i.imgur.com/K2TckTM.png)

The plugin is responsive. If there is no place on the left, it will move to the text.

![jQuery insert plugin for MediumEditor - #6 screenshot](http://i.imgur.com/uJkBT0z.png)

The image addon allows you to choose image styles and even to create custom ones.

![jQuery insert plugin for MediumEditor - #2 screenshot](http://i.imgur.com/1Rpw0Wo.png)
![jQuery insert plugin for MediumEditor - #3 screenshot](http://i.imgur.com/e0WbMPy.png)

The embeds addon support content from various sources:

![jQuery insert plugin for MediumEditor - #4 screenshot](http://i.imgur.com/97Z9MPV.png)


## Download

* Bower (recommended): ```bower install medium-editor-insert-plugin#1.0 --save```
* Manual: [Download the latest release](https://github.com/orthes/medium-editor-insert-plugin/releases)


## Quick Start

The first step is to include the plugin with all its dependencies to your code:

```html
<!-- CSS -->
<link rel="stylesheet" href="bower_components/medium-editor/dist/css/medium-editor.min.css">
<link rel="stylesheet" href="bower_components/medium-editor/dist/css/themes/default.css" id="medium-editor-theme">
<!-- Font Awesome for awesome icons. You can redefine icons used in a plugin configuration -->
<link href="http://netdna.bootstrapcdn.com/font-awesome/4.0.3/css/font-awesome.css" rel="stylesheet">
<!-- The plugin itself -->
<link rel="stylesheet" href="bower_components/medium-editor-insert-plugin/dist/css/medium-editor-insert-plugin.min.css">

<!-- JS -->
<script src="bower_components/jquery/dist/jquery.min.js"></script>
<script src="bower_components/medium-editor/dist/js/medium-editor.js"></script>
<script src="bower_components/handlebars/handlebars.runtime.min.js"></script>
<script src="bower_components/jquery-sortable/source/js/jquery-sortable-min.js"></script>
<!-- Unfortunately, jQuery File Upload Plugin has a few more dependencies itself -->
<script src="bower_components/blueimp-file-upload/js/vendor/jquery.ui.widget.js"></script>
<script src="bower_components/blueimp-file-upload/js/jquery.iframe-transport.js"></script>
<script src="bower_components/blueimp-file-upload/js/jquery.fileupload.js"></script>
<!-- The plugin itself -->
<script src="bower_components/medium-editor-insert-plugin/dist/js/medium-editor-insert-plugin.min.js"></script>
```

Initialize MediumEditor as you normally would:

```javascript
var editor = new MediumEditor('.editable');
```

Finally, you can initialize the insert plugin:

```javascript
$(function () {
    $('.editable').mediumInsert({
        editor: editor
    });
});
```

## [Documentation](https://github.com/orthes/medium-editor-insert-plugin/wiki)

- [Getting Started](https://github.com/orthes/medium-editor-insert-plugin/wiki/v1.0-Getting-Started)
- [Configuration](https://github.com/orthes/medium-editor-insert-plugin/wiki/v1.0-Configuration)
- [Upgrading from v0.3](https://github.com/orthes/medium-editor-insert-plugin/wiki/v1.0-Upgrading-from-v0.3)
- [Development & Contributing](https://github.com/orthes/medium-editor-insert-plugin/wiki/Development-&-Contributing)
- [License](https://github.com/orthes/medium-editor-insert-plugin/wiki/License)
- [Author & Contributors](https://github.com/orthes/medium-editor-insert-plugin/wiki/Author-&-Contributors)