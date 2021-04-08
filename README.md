# bevy_retro_demo

This is a simple example that uses a ron scene-file in [bevy-retro](https://github.com/katharostech/bevy_retro).

The basic idea is that you can edit a simple text source-file, and the engine can live-reload and display the initial scene. After it is loaded, you can write rust code to make things interactive.

## usage

You can run the example with this:

```
cargo run
```

Edit assets/scene.ron and watch it update

## ideas

These are some ideas that might make it easier to bundle scenes, and make complete games without a recompile

- web build & testing
- CI auto-building (for release downloads) and deploy to surge
- I'd like to add a few other types, like tilemaps
- wasm for compiled cross-platform interactions
- callback for input
- a few built-in methods like "load this scene" or "play this sound" or "trigger this animation on this thing"
- bundling assets + interaction wasm for complete cross-platform, cross-language game-system: your came can be a zip of folders
- example wasm controllers in several languages: rust, micropython, assemblyscript, lua, go, etc