# termux-api-package
Termux package containing scripts to call exposed API methods in the [Termux:API](https://github.com/termux/termux-api) app.

## Accessibility

`termux-accessibility` controls the Termux:API accessibility service:

```text
termux-accessibility dump [display-id]
termux-accessibility click x y [display-id] [duration-ms]
termux-accessibility swipe x1 y1 x2 y2 [display-id] [duration-ms]
termux-accessibility type text
termux-accessibility global-action action
termux-accessibility screenshot [display-id]
termux-accessibility list-displays
```

Display id defaults to `0`. Click duration defaults to `1` ms and swipe duration
defaults to `300` ms. Coordinates and display ids must be integers from `0` to
`2147483647`; durations must be from `1` to `60000` ms. `type` and
`global-action` each take exactly one argument; quote it to pass spaces.
Use `-h` or `--help` for usage.
