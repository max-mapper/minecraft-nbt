# minecraft-nbt

[named binary tag](http://www.minecraftwiki.net/wiki/NBT_format) parser in pure js

extracted from code originally written by @ithkuil for [mcchunkloader](https://github.com/ithkuil/mcchunkloader), turned into a module and now maintained by @maxogden

minecraft is property of Mojang AB

```javascript
var NBTReader = require('minecraft-nbt').NBTReader
var chunk = new NBTReader(chunkBinaryData).read()
// now you can access the parsed data, e.g.:
chunk.root.Level.Sections
chunk.root.Sections
// etc
```

this modules works with [minecraft-region](http://github.com/maxogden/minecraft-region) and [minecraft-chunk](http://github.com/maxogden/minecraft-chunk) and is used by [minecraft-mca](http://github.com/maxogden/minecraft-mca)

designed for use with [browserify](http://browserify.org)

# license

BSD