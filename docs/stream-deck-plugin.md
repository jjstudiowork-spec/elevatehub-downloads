# ElevateHub Stream Deck Plugin

The ElevateHub Stream Deck plugin connects keys in the Stream Deck app to
buttons configured in ElevateHub's Resolume Control workspace and ElevateFlow
presentation controls.

## Requirements

- ElevateHub running on the same computer as the Stream Deck app
- Stream Deck 7.1 or newer
- macOS 12 or newer, or Windows 10 or newer

## Setup

1. Open ElevateHub and unlock your Team member profile.
2. Open **Operator Workspace**, then open **Resolume Control**.
3. In the Stream Deck app, drag **ElevateHub Button** onto a key for Visual
   Control, or **ElevateFlow Button** for Flow.
4. In ElevateHub, assign that Stream Deck key to a Resolume Control button.
5. Confirm that the Property Inspector says **Synced**.

Each button can use its own background and text colours, any font installed on
the ElevateHub computer, font weight, and italic or uppercase text. Text is
automatically sized and centred for reliable key layouts. Appearance changes are included in Set exports and update on
Stream Deck hardware and Stream Deck Mobile automatically.

Keys also support built-in icons, optimized custom images, text/icon display
modes, brightness control, reusable style presets, copy/paste styling, and an
automatic contrast warning. A finished style can be applied across a Set
without changing any of its assigned actions.

When ElevateHub is closed or disconnected, the key displays the ElevateHub
logo. Open ElevateHub and Resolume Control to reconnect automatically.

## Troubleshooting

- Keep ElevateHub and Stream Deck running on the same computer.
- Confirm that only one ElevateHub instance is open.
- Remove and re-add the Stream Deck action if its device layout changed while
  Stream Deck was offline.
- Restart the Stream Deck app after installing a development build.

The plugin communicates only with ElevateHub or ElevateFlow over
`127.0.0.1:47825`. It does not send button assignments or account information
over the internet.

## Releasing a plugin update

When the plugin itself changes, bump both its `package.json` version and the
plugin manifest version. A normal `npm run publish:all` release now packages
the plugin, attaches it to the public release, and updates the download on the
ElevateHub website automatically.

For support, open an issue in the
[ElevateHub support tracker](https://github.com/jjstudiowork-spec/elevatehub-downloads/issues).
