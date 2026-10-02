# Ryquex Review Viewer — English v2

A portable Windows x64 catalogue and review tool for item bases, modifiers and passive skills. English is the default interface language. All edits are local review proposals: the owner's working Ryquex project is never changed automatically.

## Download and run

1. Download `Ryquex-ReviewViewer-Windows-x64-v2.0-English.zip` from [Releases](https://github.com/iamcoolstory/RyquexViewer/releases).
2. Extract the **entire ZIP** into a separate folder. Do not run the application from inside the archive.
3. Run `Ryquex.Viewer.exe`. Keep the `Public` folder beside the executable.
4. Your default browser will open the Viewer at a local `127.0.0.1` address.

Requirements: Windows x64 and a modern browser, such as Microsoft Edge or Google Chrome. No internet connection, Ryquex installation or separate .NET installation is required after downloading.

The executable is not digitally signed yet. Windows SmartScreen may show a warning. Only run the archive obtained from the trusted repository.

To stop the application, click **Exit** in the Viewer header. Closing the browser tab alone does not stop the local server.

## Pages

- **Bases** — browse item types and bases with their images. Search by base name or ID.
- **Mods** — filter by item type and attributes, search modifiers, expand families and inspect Implicit, Prefix, Suffix, Craft Prefix, Craft Suffix and Enchantment. Unassigned, Assigned and Regular / Advanced / Ultimate sections are available.
- **Passive Skills** — expandable thematic cards with Minor, Medium, Major and Supreme tiers. Searching `major | supreme` matches either query.
- **▱ Preview interface** — switch between the interface overview, Inventory and Skill Hub using the adjacent selector.

## Inventory and generation

Open **▱ → Inventory**. **Generate 15 items** creates random items. Selecting a specific item type switches to browsing its bases; the arrows move between pages.

Items can be dragged or attached to the cursor with a left click. In normal mode, right-click equips or unequips an item. In developer mode, right-click opens the visual editor.

Use **Show settings / Hide settings** for interface dimming controls. Each quick-access slot has its own clear button.

## Review and adjust a base

1. In **Bases**, select an item type and locate a base.
2. Click **Edit in inventory** to open that base in the developer editor.
3. Alternatively, enable **Developer** in Inventory and right-click an item.
4. Adjust horizontal mirroring, rotation, scale, horizontal/vertical offsets, pixel width/height and drawing over the frame.
5. Use **Edit card appearance** to adjust its item-card image. Slot and card settings are independent.
6. **Copy slot settings** copies the slot appearance into the card appearance.

Changes save automatically. **Save changes** is also available.

### Editor shortcuts

- `↑` / `↓` — select the parameter to edit.
- `←` / `→` — adjust the value or toggle a checkbox.
- `Shift` — use a larger adjustment step.
- `\` — switch between slot and card editing.
- `]` — copy slot settings into the card.

**Preview inventory** returns to the inventory display. **BAD BASE** flags an unsuitable base and lets you add a comment. **Clear flag** removes the flag from the Bases page.

## Change log and sharing feedback

Click **Log** to inspect your changes. The journal keeps **one final entry per setting**, not a separate entry for every slider movement. Slot and card appearances are independent entries for the same base. Editing the same setting again updates its entry.

Click **Export log** to download `Ryquex-feedback.json`. Send this file to the owner for review and application to the source Ryquex project. It includes stable IDs, original/final appearance settings, base feedback and modifier/passive proposals.

Changes are stored outside the application folder:

```text
%LOCALAPPDATA%\RyquexViewer\<bundle ID>\
```

They survive closing and restarting the Viewer. A new catalogue snapshot can have its own profile, so export your feedback before switching releases. Older verbose journals are compacted automatically and backed up locally.

## Updating

Export your current feedback, click **Exit**, download the new release and extract it into a new folder. Run the executable from that folder. Do not replace files while the Viewer is running.

English v2 is a separate release. Russian v1.1 remains available in the release history. Export feedback from the old version before switching; its local profile is not deleted.

## Privacy and scope

Only the approved catalogue snapshot, artwork and Viewer components are included. The owner's private notes, PSD source files, game source code, keys and working Ryquex settings are excluded.

The Viewer does not publish edits or connect to the owner's project. Visible descriptions, images and the Viewer's own HTML/JavaScript can be copied by recipients. User-written comments are stored verbatim and are not automatically translated.

## Troubleshooting

- Confirm that the entire archive was extracted and `Public` is beside the EXE.
- Confirm that Windows is x64 and a default browser is configured.
- Stop an old Viewer using **Exit** before starting a different release.
- If saving fails, stop editing, export any available feedback and report the error to the owner.
