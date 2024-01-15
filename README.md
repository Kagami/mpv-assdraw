# mpv-assdraw

Port of [assdraw.lua](https://github.com/mpv-player/mpv/blob/master/player/lua/assdraw.lua) to TypeScript.

## Install

```bash
npm i mpv-assdraw
```

## Usage

```javascript
import AssDraw from "mpv-assdraw";

const { width, height } = mp.get_osd_size();
const ass = new AssDraw();
ass.new_event();
ass.append("test");
mp.set_osd_ass(width, height, ass.text);
```
