# Open OTT Play

Open-source IPTV/OTT playback for set-top boxes, smart TVs, and the browser.
FOSS revival of a classic STB web player — rebuilt module by module in TypeScript,
compatible back to ES5-era hardware.

## Projects

### [ottplay-foss](https://github.com/open-ott-play/ottplay-foss)

The main project: a browser-based IPTV/OTT player that runs on 24 device families —
Samsung Tizen, LG webOS, Panasonic Viera, Infomir MAG, Dune HD, Android TV, and more.

- **Playback** — HLS, DASH, and plain HTTP streams via hls.js and Shaka Player
- **EPG** — XMLTV program guide with fuzzy channel matching and time-shift support
- **Providers** — M3U playlists, Xtream Codes API, Stalker middleware
- **Push commands** — remote control over HTTP: switch channel/provider, popups, volume
- **Per-device routing** — UUID-based addressing for multi-room setups
- **Local proxy** — optional command server for fully local automation (Home Assistant, Node-RED)
- **21 languages**, per-device key mappings, parental controls, favorites, archive mode

```bash
git clone https://github.com/open-ott-play/ottplay-foss.git
cd ottplay-foss && npm install && npm run build
python3 server.py 8080   # serve + EPG proxy
```

## Contributing

PRs welcome — CI runs CodeQL on every push, commits must be signed.
UI, channels, settings, providers, localization, and polyfills are all open ground;
translations are especially appreciated.

## License

Everything here is [MIT](https://github.com/open-ott-play/ottplay-foss/blob/main/LICENSE).
