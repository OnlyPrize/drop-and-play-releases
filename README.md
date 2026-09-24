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

Dropped files are uploaded to `music/<playlist name>/` in your User Data. You can
change the folder in the module settings. An upload never replaces a file that is
already there.

In **Shuffle** mode the order is random, so dropped tracks go to the end and
tracks cannot be dragged. Switch to **In order** to arrange them.

## License

Free to use in your own games. Redistribution, resale and republishing are not
permitted — see [LICENSE](LICENSE).
