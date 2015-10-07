Sublime Text 3 Configuration
---

Download [Sublime Text 3](http://www.sublimetext.com/3)

Installation von [PackageControl](https://packagecontrol.io/)



## Theme

[Cobalt 2](https://github.com/wesbos/cobalt2) von [@wesbos](https://github.com/wesbos)


## User Settings

```
{
    "caret_extra_bottom": 3,
    "caret_extra_top": 3,
    "caret_extra_width": 2,
    "color_scheme": "Packages/Theme - Cobalt2/cobalt2.tmTheme",
    "theme": "Cobalt2.sublime-theme",
    "ensure_newline_at_eof_on_save": true,
    "font_size": 12.0,
    "highlight_line": true,
    "ignored_packages":
    [
        "Vintage"
    ],
    "open_files_in_new_window": false,
    "overlay_scroll_bars": "enabled",
    "tab_size": 2,
    "trailing_spaces_file_max_size": 1000,
    "trailing_spaces_highlight_color": "invalid",
    "translate_tabs_to_spaces": true,
    "trim_trailing_white_space_on_save": true,
    "word_wrap": true
}
```



## Packages
---

* [Sass](https://packagecontrol.io/packages/Sass)
* [Emmet](https://packagecontrol.io/packages/Emmet)
* [Apache​Conf](https://packagecontrol.io/packages/ApacheConf.tmLanguage) - Syntax Highlighting für .htaccess
* [Editor​Config](https://packagecontrol.io/packages/EditorConfig) - Helps developers maintain consistent coding styles between different editors
* [BracketHighlighter](https://packagecontrol.io/packages/BracketHighlighter) - Bracket and tag highlighter
* [Side​Bar​Enhancements](https://packagecontrol.io/packages/SideBarEnhancements)



## Packages Settings
---


### Emmet


```
{
  "css_completions_scope": "source.css - meta.selector.css - meta.property-value.css, source.scss - meta.selector.css - meta.property-value.css, source.less - meta.selector.css - meta.property-value.css, source.sass - meta.selector.css - meta.property-value.css",
  "preferences": {
    "sass.propertyEnd": ";"
  }
}
```


## Snippets
Erstellen in Sublime Text unter `Tools` > `New Snippet`

Die Dateien haben die Endung `.sublime-snippet` und liegen unter folgendem Pfad (OSX)
`user/Library/Application Support/Sublime Text 3/Packages/User/`


### Breakpoint Sass Mixin 
`breakpoint.sublime-snippet`

```
<snippet>
  <content><![CDATA[
@include breakpoint(${1:}) {
  ${2:}
}
]]></content>
  <!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
  <tabTrigger>bp</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <scope>source.sass</scope>
</snippet>
```

### Kommentar Block
`kommentar-block.sublime-snippet`

```
<snippet>
  <content><![CDATA[
//*******************************************************************************
// ${1:Beschreibung}
//*******************************************************************************
]]></content>
  <!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
  <tabTrigger>kommentar-block</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope>source.python</scope> -->
</snippet>
```

### console.log();
`console-log.sublime-snippet`

```
<snippet>
  <content><![CDATA[
console.log($1);
]]></content>
  <tabTrigger>con</tabTrigger>
</snippet>
```


