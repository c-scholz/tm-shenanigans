# How to use the Snippets

The snippets provided can be used inside custom code for Nightbot commands.

>Note:
>These snippets do not work out of the box. They are supposed to be used in a context by persons that can write custom code used e.g. in Nightbot commands.

# regex-text_formatting

Example usage:

```
// filter out all text formatting from a map name
const r = /(\$[0-9a-fA-F]{3})|(\$[inowstz$]{1})|(\$l\[.*?\])/g

const cleanMapName = cleanMapName.replaceAll(r,'')
```
