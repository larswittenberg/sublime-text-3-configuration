Sublime Text 3 Configuration
---

Download [Sublime Text 3](http://www.sublimetext.com/3)

Installation von [PackageControl](https://packagecontrol.io/)


## Theme

[Cobalt 2](https://github.com/wesbos/cobalt2) von [@wesbos](https://github.com/wesbos)


## Font
[Hack | A typeface designed for source code](http://sourcefoundry.org/hack/)


## User Settings

```json
{
	"caret_extra_bottom": 3,
	"caret_extra_top": 3,
	"caret_extra_width": 2,
	"color_scheme": "Packages/Theme - Cobalt2/cobalt2.tmTheme",
	"draw_white_space": "all",
	"ensure_newline_at_eof_on_save": true,
	"font_face": "Hack",
	"font_size": 13.0,
	"highlight_line": true,
	"ignored_packages":
	[
		"Vintage"
	],
	"open_files_in_new_window": false,
	"overlay_scroll_bars": "enabled",
	"tab_size": 2,
	"theme": "Cobalt2.sublime-theme",
	"trailing_spaces_file_max_size": 1000,
	"trailing_spaces_highlight_color": "invalid",
	"translate_tabs_to_spaces": true,
	"trim_trailing_white_space_on_save": true,
	"word_wrap": true,
	"show_encoding": true
}
```


## Key Bindings User

```json
[
  // Fix End of line
  { "keys": ["super+right"], "command": "move_to", "args": {"to": "hardeol", "extend": false} }
  // Fix Beginning of line
  ,{ "keys": ["super+left"], "command": "move_to", "args": {"to": "hardbol", "extend": false} }
  // Fix end of line + select
  ,{ "keys": ["super+shift+right"], "command": "move_to", "args": {"to": "hardeol", "extend": true} }
  // Fix beginning of line + select
  ,{ "keys": ["super+shift+left"], "command": "move_to", "args": {"to": "hardbol", "extend": true} }
]
```

[Proper go to end of line with Sublime Text](http://wesbos.com/sublime-text-end-of-line-wrap/)


## Packages
`Command Palette` > `List Packages`

* [Apache​Conf](https://packagecontrol.io/packages/ApacheConf.tmLanguage) - Syntax Highlighting für .htaccess
* [BracketHighlighter](https://packagecontrol.io/packages/BracketHighlighter) - Bracket and tag highlighter
* [Editor​Config](https://packagecontrol.io/packages/EditorConfig) - Helps developers maintain consistent coding styles between different editors
* [Emmet](https://packagecontrol.io/packages/Emmet)
* [Package Control](https://packagecontrol.io/installation)
* [Sass](https://packagecontrol.io/packages/Sass)
* [Side​Bar​Enhancements](https://packagecontrol.io/packages/SideBarEnhancements)
* [Theme - Cobalt 2](https://github.com/wesbos/cobalt2)
* [TypoScript Syntax Highlighter](https://packagecontrol.io/packages/TypoScript)
* [MJML Syntax Highlighter](https://packagecontrol.io/packages/MJML-syntax)



## Packages Settings

### Emmet
Menü `Sublime Text` > `Preferences` > `Package Settings` > `Emmet` > `Settings - User`

```json
{
  "css_completions_scope": "source.css - meta.selector.css - meta.property-value.css, source.scss - meta.selector.scss - meta.property-value.scss, source.less - meta.selector.css - meta.property-value.css, source.sass - meta.selector.css - meta.property-value.css",
  "preferences": {
    "sass.propertyEnd": ";"
  }
}
```


## Snippets

Erstellen in Sublime Text unter `Tools` > `New Snippet`

Die Dateien haben die Endung `.sublime-snippet` und liegen unter folgendem Pfad (OSX)
`Benutzer/[Benutzername]/Library/Application Support/Sublime Text 3/Packages/User/`
(Sublime Text Menü → Preferences → Browse Packages...)


#### Breakpoint Sass Mixin
`breakpoint.sublime-snippet`

```html
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

#### print_r() Ausgabe
`print_r.sublime-snippet`

```html
<snippet>
  <content><![CDATA[
echo '<pre>';
print_r(${1:});
echo '</pre>';
]]></content>
  <!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
  <tabTrigger>pre</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <scope>source.php</scope>
</snippet>
```


#### Kommentar Block
`kommentar-block.sublime-snippet`

```html
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

#### console.log();
`console-log.sublime-snippet`

```html
<snippet>
  <content><![CDATA[
console.log($1);
]]></content>
  <tabTrigger>con</tabTrigger>
</snippet>
```


