GAMER & STREAMER INSTALLER
==========================
A friendly installer window for gamers and streamers. Click the programs you want, press one button, and they download and install quietly through Windows' built-in package manager (winget).

HOW TO USE
1. Double-click "Gamer Installer.bat". A window opens.
   (Use "Gamer Installer (Admin).bat" to approve administrator permission ONCE instead of for every program.)
2. Click the programs you want. GREEN = will be installed. RED = skipped.
   - QUICK PICKS: one click adds a ready-made group of programs. Quick picks only ADD programs;
     use "Clear everything" to start over.
   - The search box finds programs by name or by what they do. Press Esc to clear it.
   - "All" / "None" on each category box picks or clears that whole group.
   - "Installed on this PC" means you already have it, so you can leave it red.
   - "Update available" means a newer version exists.
3. Press the big green "Install selected" button and confirm.
   Programs install one after another with a progress bar and a log. "Stop after this program"
   finishes the current program and skips the rest.
4. Some programs may show a Windows permission (UAC) prompt. That is normal - choose Yes.

MORE FEATURES
- Save my picks / Load picks: save your selection to a file and load it on another PC.
- Update installed programs: appears when programs you already have have a newer version.
- Retry failed: if some programs fail, the log says why in plain words and you can retry just those.
- Install order: programs that others depend on go first (for example WSL before Docker).
- Restart notice, and a saved log of every run in %LOCALAPPDATA%\PCInstallers\logs.
- If winget is missing, the window says so and offers a button to get it from the Microsoft Store.

REQUIREMENTS
- Windows 10 (1809 or newer) or Windows 11 with winget ("App Installer"), already on most PCs.
- An internet connection. Nothing is installed until you press the green button and confirm.

TO ADD OR REMOVE A PROGRAM
Edit gamer-catalog.json. Each entry needs: category, name, id (the winget ID), source ("winget" or "msstore"),
and description. Find a winget ID by running:  winget search <name>
Quick picks are in gamer-presets.json; the programs that start ticked are "starter" in gamer.config.json.

NOTES
- Emulators do not include games or console BIOS files. You need your own legally obtained copies.
- Logos come from Simple Icons (simpleicons.org, CC0) and from each program's own website or project page.
  Brand logos belong to their owners and are shown only to identify each program. Programs without a
  findable logo show a colored letter badge.