# Drop & Play

A Foundry VTT module that makes running music easier: drop audio files or whole
folders straight into a playlist, and rearrange tracks while the music keeps playing.

> ลากไฟล์เพลงหรือทั้งโฟลเดอร์ลง playlist ได้เลย และสลับลำดับเพลงได้ระหว่างที่เพลงกำลังเล่น

## Install

In Foundry's **Add-on Modules → Install Module**, paste this manifest URL:

```
https://github.com/OnlyPrize/drop-and-play-releases/releases/latest/download/module.json
```

Requires Foundry VTT v13 or v14. Works with any game system.

## Use

Open the **Playlists** tab and press **Drop & Play** (Gamemasters only).

| Do this | What happens |
|---|---|
| Drop a folder on the left column | A new playlist named after the folder, with every audio file in it |
| Drop files onto a playlist's name | They are added to the end of that playlist |
| Drop files between two tracks | They are inserted right there |
| Drag a track up or down | The order changes — the track that is playing keeps playing |
| Click a track's play button | That track plays now; click again to pause |
| Click a track's 🔁 button | That track loops until you click it again |

Dropped files are uploaded to a folder named after the playlist inside `music/` in
your User Data — "Tavern Songs" goes to `music/tavern-songs/`. A name with no Latin
letters or digits, such as a Thai one, uses the playlist's ID as the folder name.
You can change `music` to another folder in the module settings. An upload never
replaces a file that is already there.

In **Shuffle** mode the order is random, so dropped tracks go to the end and
tracks cannot be dragged. Switch to **In order** to arrange them.

### Crossfade

When you start a playlist from the Drop & Play window, the music already playing
on the same channel fades out while the new playlist fades in. Set how many
seconds it takes (0–10, default 3) in the **Crossfade** box under the playlist
list; 0 turns it off and lets both keep playing. Soundboard playlists are never
stopped by a crossfade.

### Sound effects pad

Press **Sound Effects** (in the Playlists tab or the Drop & Play window) to open a
small pad you can keep on screen during play.

| Do this | What happens |
|---|---|
| Click ⚡ on a track in Drop & Play, or drag a track onto the pad | It becomes a button on the pad |
| Click a pad button | Everyone hears that sound once, over the music, at their Environment volume |
| Hover a pad button, click ⌨, then press a key | That key (with Ctrl, Shift or Alt if you like) plays the sound. Esc cancels, Backspace clears |
| **Stop all effects** | Stops every pad sound that is still playing, for everyone |

Hotkeys work whenever you are in the world, even with the pad closed, but not
while you are typing in chat or a text box. If a key is also a Foundry shortcut
(W moves up, for example), the pad tells you and takes that key over.

## License

Free to use in your own games. Redistribution, resale and republishing are not
permitted — see [LICENSE](LICENSE).
