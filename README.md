# FiveM Radio

This resource allows you to integrate your own radios in place of the original radios.
It's fully written in JavaScript and uses resource metadata for its configuration.

## Features

* Radio wheel
* Audio file
* Audio stream
* No dependency
* Easy configuration

## Showcase

Video showing Los Santos Rock Radio replaced by a WebRadio and Non-Stop-Pop FM replaced by a song:
[![Showcase](https://cf-e2.streamablevideo.com/image/6hrhp.jpg)](https://streamable.com/6hrhp "Showcase")

## Known bugs and limitations

* `citizen-legacy-net-resources`
* Vehicles still emits low sound of the original radio
* No automatic stream recovery in case of network error
* No MPEG, MP3 or AAC support as CEF only supports open formats

## Configuration

For each custom radio, add this line in `_resource.lua`:
```lua
supersede_radio "[RADIO_NAME]" { url = "[RADIO URL]", volume = 0.5 }
```

You can find the list of radio names in [`data.js`](data.js) and a full example in [`__resource.lua`](__resource.lua).

## Tips

Stream a modified `hud.ytd` (`gtav_radio_stations_texture_512`) file to replace radio logos.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.