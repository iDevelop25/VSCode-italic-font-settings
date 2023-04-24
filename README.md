# VSCode italic font settings

*Add this to settings.json (`cmd ,`):*
```
{
  "editor.fontFamily": "Operator Mono, Fira Code iScript, Menlo, Monaco, 'Courier New', monospace",
  "editor.fontLigatures": true,
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": [
          //following will be in italic
          "comment",
          "entity.name.type.class", //class names
          "constant", //String, Number, Boolean…, this, super
          "storage.modifier", //static keyword
          "storage.type.class.js", //class keyword
          "keyword", //import, export, return…
        ],
        "settings": {
          "fontStyle": "italic"
        }
      },
      {
        "scope": [
          //following will be excluded from italics (VSCode has some defaults for italics)

          "invalid",
          "keyword.operator",
          "constant.numeric.css",
          "keyword.other.unit.px.css",
          "constant.numeric.decimal.js",
          "constant.numeric.json"
        ],
        "settings": {
          "fontStyle": ""
        }
      }
    ]
  },
}
```

## Resources
https://www.cufonfonts.com/font/operator-mono
https://github.com/kencrocken/FiraCodeiScript
https://github.com/tonsky/FiraCode
```
"editor.fontFamily": "Fira Code",
"editor.fontLigatures": true`
```
https://github.com/kosimst/FiraFlott
