<div align="center">
  <img src="src-tauri/icons/elevatehub-master.png" alt="ElevateHub" width="128" />
  <h1>ElevateHub</h1>
  <p><strong>One place for your live production tools, studios, and team.</strong></p>
  <p>
    <a href="https://github.com/jjstudiowork-spec/elevatehub-downloads/releases/latest">Download ElevateHub</a>
    ·
    <a href="docs/stream-deck-plugin.md">Stream Deck setup</a>
    ·
    <a href="https://github.com/jjstudiowork-spec/elevatehub-downloads/releases">Release notes</a>
  </p>
</div>

ElevateHub brings presentation, media, operator, and production tools into one connected desktop experience. Open ElevateFlow, arrange an Operator Workspace, manage studios, and connect production computers from the Hub.

## Download And Install

Download the latest version from the [ElevateHub releases page](https://github.com/jjstudiowork-spec/elevatehub-downloads/releases/latest).

### macOS

1. Download the universal `.dmg` file.
2. Open it and drag **ElevateHub** into **Applications**.
3. Open ElevateHub from Applications.

ElevateHub is not currently notarized through Apple's paid Developer Program. If macOS blocks the first launch, open Terminal and run:

```bash
xattr -rd com.apple.quarantine /Applications/ElevateHub.app
```

Then open ElevateHub again. The universal build supports Apple silicon and Intel Macs.

### Windows

1. Download the Windows `x64-setup.exe` file.
2. Run the installer.
3. Open **ElevateHub** from the Start menu or desktop shortcut.

Windows may display a SmartScreen notice because the installer is not currently code-signed. Confirm that the installer came from the official ElevateHub downloads repository before continuing.

## First Launch

1. Sign in or create your ElevateHub account.
2. Complete the first-time setup.
3. Select your Team member profile.
4. Enter your four-digit PIN when requested.
5. The Launcher will show the studios and tools available to your account.

Team administrators can add members, assign roles, and manage member access from **Profile**.

## ElevateFlow

ElevateFlow is the primary presentation studio. Open it from the Launcher and use it to:

- Create libraries, songs, slides, and presentations.
- Import PowerPoint presentations and add images or videos.
- Arrange text, backgrounds, media, and themes in Edit mode.
- Configure audience, stage, and windowed outputs.
- Run presentations from Show mode.
- Send or receive presentation content across the local network.
- Use LTC timecode and other production tools.

Your libraries and presentation changes are saved automatically. ElevateFlow remains independently launchable after it has been installed by ElevateHub.

## Operator Workspace

Operator Workspace keeps production information beside your main production software. Choose either:

- **Side layout:** a portrait workspace positioned at the side of the display.
- **Top layout:** a compact landscape workspace positioned across the top.

Available tools include Planning Center, Resolume Control, service countdowns, and the Timing Monitor. Workspace layouts can be saved and restored for different operators or services.

## Resolume And ProPresenter Timing

The Timing Monitor can connect multiple production computers over the same local network.

1. Choose the role of each computer: **Resolume**, **Middle**, or **ProPresenter**.
2. Choose whether the workflow uses a middle computer.
3. On the Resolume computer, configure the Resolume host, port, layer, and column.
4. On the ProPresenter computer, discover and connect to the ElevateHub computer on the network.
5. Select the ProPresenter timers that should receive updates.
6. Use **Sync** to copy the active clip's remaining time to only the selected timers.

Wi-Fi and Ethernet are both supported. Ethernet is recommended for the most stable live-production connection. Allow ElevateHub, Resolume, and ProPresenter through the operating system firewall.

## Stream Deck

The ElevateHub Stream Deck plugin mirrors buttons configured in Resolume Control. Keys receive their labels, colors, actions, set navigation, and device positions from ElevateHub.

1. Install the ElevateHub Stream Deck plugin.
2. Open ElevateHub and unlock your Team member profile.
3. Open **Operator Workspace**, then **Resolume Control**.
4. Drag **ElevateHub Button** onto a key in the Stream Deck app.
5. Assign that key from Resolume Control.
6. Confirm that the Property Inspector reports **Synced**.

See the complete [Stream Deck setup and troubleshooting guide](docs/stream-deck-plugin.md).

## Updates And Studios

ElevateHub checks for signed updates and shows an update window when a new version is available. Choose **Install Update** and allow the app to restart when installation finishes.

Studios can be installed, opened, updated, and removed from ElevateHub. Installed studios remain separate apps, so they can also be opened directly from Applications or the Windows Start menu.

## Troubleshooting

### A studio will not open

- Confirm the studio is installed in ElevateHub.
- Try opening it directly from Applications or the Start menu.
- Restart ElevateHub after installing or updating a studio.

### A network tool cannot find another computer

- Confirm both computers are on the same network.
- Prefer Ethernet during live events.
- Allow the apps through macOS or Windows firewall settings.
- Confirm the displayed IP address and port belong to the correct computer.
- Keep ElevateHub running even when another app is in the foreground.

### Stream Deck shows the ElevateHub logo

The logo is the disconnected state. Open ElevateHub and Resolume Control on the same computer as the Stream Deck app. The keys reconnect and restore their assigned appearance automatically.

### An update cannot be installed

- Confirm the computer has internet access and enough free storage.
- Restart ElevateHub and try again.
- Download the latest installer manually from the [official releases page](https://github.com/jjstudiowork-spec/elevatehub-downloads/releases/latest) if necessary.

## Production Checklist

Before using ElevateHub at a live event:

- Test every output and production computer.
- Confirm display routing and audio playback.
- Verify Resolume and ProPresenter API access.
- Check firewall permissions and network connectivity.
- Trigger every important Stream Deck key.
- Keep a backup plan for critical presentation and playback workflows.

## Privacy And Availability

ElevateHub is under active development. ElevateFlow is the primary released studio; other studios and experimental tools may remain restricted while they are being built.

The Stream Deck plugin communicates with ElevateHub locally and does not collect analytics or personal information. See the [Stream Deck privacy information](docs/stream-deck-privacy.md).

Copyright © 2026 ElevateHub. All rights reserved.
