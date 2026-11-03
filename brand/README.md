# Brand images

- `avatar.png`: organization avatar, 500×500
- `cli.png`, `ping-action.png`, `examples.png`: repository social previews, 1280×640

They are rendered from `avatar.html` and `card.html` (name, lead and cmd come from the query string) with headless Chrome:

```sh
chrome --headless=new --hide-scrollbars --force-device-scale-factor=1 --virtual-time-budget=6000 \
  --window-size=1280,640 --screenshot=cli.png "file://$PWD/card.html?name=cli&lead=...&cmd=..."
```

Colors: navy `#0D1326`, pulse blue `#8FB4FF`, missed beat red `#FF5A63`. Fonts: Geologica and JetBrains Mono.
