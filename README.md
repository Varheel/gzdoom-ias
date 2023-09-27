# GZDoom - Steam Workshop Support

This is a fork of [GZDoom](https://github.com/ZDoom/gzdoom) that automatically loads mods from a Steam Workshop folder. It's for Steam games that run on GZDoom.

The mod folder is configured via `ModConfig.json`, which is placed in the same folder as `gzdoom.exe`.
The `ModFolder` property specifies the relative path to the Steam Workshop folder.
`FileTypes` is an array that specifies which types of files to load.
The game will recursively search the `ModFolder` and load all WADs, PK3s, etc.

Example `ModConfig.json` file:
```
{
	"ModFolder": "../../workshop/content/2477140",
	"FileTypes":
	[
		".wad",
		".pk3",
		".pk7",
		".pkz",
		".zip",
		".7z"
	]
}
```
