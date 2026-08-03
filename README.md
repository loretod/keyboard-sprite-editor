# Keyboard Sprite Editor for MakeCode Arcade

A fully keyboard-operable pixel art editor built to make sprite and background creation in [MakeCode Arcade](https://arcade.makecode.com/) accessible to students who can't rely on a mouse.

**Live demo:** [Keyboard Sprite Editor](https://loretod.github.io/keyboard-sprite-editor/)

## Why this exists

MakeCode Arcade's block editor has made real strides on keyboard accessibility. Its built-in sprite/image editor, however, still depends on mouse-driven, click-and-drag pixel painting. For students with physical disabilities who can't reliably control a mouse, that leaves a gap right at the point where a lot of the fun happens: designing what things look like.

This tool closes that gap. Every action needed to design a sprite or background — choosing a size, picking a color, painting pixels, exporting the result — is reachable from the keyboard alone, and every state change is announced for screen reader users too.

## Features

- **Six canvas sizes** matching real MakeCode Arcade gallery sprite dimensions — 16×16, 32×32, 48×48, 24×16, and 16×24 — plus a full 160×120 **Background** canvas matching the actual MakeCode Arcade screen resolution.
- **The official 16-color MakeCode Arcade palette**, presented as an accessible color radio-group navigable by row and column.
- **Full keyboard drawing controls** — arrow keys to move, Space/Enter to paint, Backspace/Delete to erase, Shift+Arrow to jump five cells at a time, Home/End and Ctrl+Home/Ctrl+End to jump across a row or the whole canvas.
- **Section shortcuts** — press `1`–`4` anywhere on the page to jump straight to Canvas size, Active color, Draw, or Export. The active section is highlighted with a background change, a border change, and a text badge (never color alone), and the highlight passes WCAG AA contrast.
- **One-click, fully automatic export** — generates a MakeCode-compatible `img\`...\`` literal and copies it to the clipboard the moment you click the button, with a visible on-screen fallback for the rare case where automatic copying isn't available in the browser.
- Live screen-reader announcements of cursor position, painted cells, and section changes; visible focus indicators throughout; no drag gestures anywhere in the tool.

## Using the tool

1. Pick a canvas size.
2. Pick an active color.
3. Move around the grid with the arrow keys and press Space or Enter to paint. Backspace or Delete erases.
4. Click **Copy MakeCode code**. Paste the result over the image inside a sprite's `img\`...\`` block in the MakeCode JavaScript editor.

## Keyboard reference

| Key | Action |
|---|---|
| `1`–`4` | Jump to a section (canvas size / active color / draw / export) |
| Arrow keys | Move the drawing cursor, or move through the color palette by row/column |
| Shift + Arrow | Move the drawing cursor five cells at a time |
| Home / End | Jump to the start / end of the current row |
| Ctrl+Home / Ctrl+End | Jump to the top-left / bottom-right corner of the canvas |
| Space / Enter | Paint the current cell with the active color |
| Backspace / Delete | Erase the current cell (make it transparent) |

## Status

This is an early-stage teaching tool built for a coding curriculum aimed at upper elementary and middle school students. It has not yet been tested end-to-end with assistive technology users. Feedback and issue reports are welcome through the issues section of this repo.

## Attribution

This tool was built with the assistance of [Claude](https://claude.com), Anthropic's AI model.

## License

This project is licensed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**.

See [LICENSE.md](./LICENSE.md) for the summary, or the [full legal text](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode) at Creative Commons.