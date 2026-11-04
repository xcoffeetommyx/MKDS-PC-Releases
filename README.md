# Mario Kart DS for PC (beta)

The original **Mario Kart DS (USA)** as a Windows game, with both screens,
controller support, sharper 3D and online races on community servers.

**No game is included.** You build it yourself from your own Mario Kart DS
ROM. This page only has the builder and the server.

## Downloads

Get them from the **Releases** page (on the right):

- **`MKDS-Vanilla-PC-Setup-1.0.0-beta.1.zip`**: the builder. Everyone needs it.
- **`MKDS-Room-Server-1.3.1.zip`**: the online server. Only the person
  hosting needs it.

## What you need

- Windows 10 or 11 (64-bit)
- Internet for the first build, and about 6 GB of free space
- Your own **Mario Kart DS (USA)** ROM (`.nds`). Other regions and modified
  ROMs are refused.

## 1. Build the game

1. Extract `MKDS-Vanilla-PC-Setup-1.0.0-beta.1.zip`.
2. Double-click **`Launch.cmd`**. The builder opens.
   (If Windows shows a blue warning: **More info**, then **Run anyway**.)
3. Under **YOUR ROM**, press **Browse...** and pick your `.nds` file.
4. Under **GAME FOLDER**, press **Browse...** and pick where the game
   should be built, for example `C:\Users\you\Games\Mario Kart DS`.
5. Press **Build game** and wait. The first build downloads its tools,
   so it can take a while (up to an hour or more on slower PCs).
6. When it's done, say **Yes** to the desktop shortcut.

## 2. Play

Start the game any of these ways:

- the **Mario Kart DS** shortcut on your desktop,
- the **Play** button in the builder (open `Launch.cmd` again),
- or **`Mario Kart DS.exe`** in the game folder you picked.

**Controls:** controllers work right away. Keyboard: arrows = D-pad,
Z/X = A/B, A/S = Y/X, Q/W = L/R, Enter = Start, Backspace = Select. Click
the bottom screen with the mouse. **Esc** opens the settings menu (buttons,
3D quality, your online name, server). **Alt+Enter** is fullscreen.

## 3. Play online

1. In the game, press **Esc**, open **Online**, select **Enter address**
   and press **Enter**.
2. Type the address of the server (the host gives it to you, for example
   `203.0.113.5`) and press **Enter**. Then close the menu with **Esc**.
   - On the same home network as the server, skip this: the game finds
     it by itself.
3. In the game's main menu, choose **Nintendo WFC** and connect, like on a
   DS. **Worldwide** races everyone on the server; **Friends** races the
   people whose friend codes you added.

Up to 4 players per race. Everyone needs the same version of the game.

## 4. Host a server

Only one person needs to do this.

1. Extract `MKDS-Room-Server-1.3.1.zip`.
2. Double-click **`Start-Server.cmd`**. A terminal window opens. Keep it
   open while people play; close it to stop the server.
3. If Windows Firewall asks, press **Allow** (tick both private and
   public networks).
4. Make sure friends can reach you on **UDP port 29999**:
   - The window says *"opened UDP port 29999 automatically (UPnP)"*: you're
     done.
   - It says UPnP is off or failed: turn on **UPnP** in your router's
     settings, **or** add a port forward in your router: **UDP**, port
     **29999**, to this PC (the window shows this PC's address, like
     `192.168.1.20`).
5. Give your friends your **internet address**. The window shows it, or
   search "what is my IP". They type it in **Esc > Online > Enter address**.

People on your home network, and you, don't need the address: the game
finds the server by itself. More help (and what to do if port forwarding
can't work) is in `HOSTING.md` inside the server zip.

## Updating

Download the new version, open its `Launch.cmd`, pick your ROM and the
**same game folder**, and press **Build game**. Your save is kept.
**Previous version** in the builder goes back if needed.

## Problems?

Open an issue in the **Issues** tab. Say what happened, and attach the
builder's error log (**Open error log**) or `logs\game-log.txt` from your
game folder. Never upload your ROM, your save or the built game.

The full guide is `README.md` inside the setup zip.

---

*Fan project, not affiliated with Nintendo. Mario Kart belongs to its
rights holders. Free and non-commercial. Don't share the built game or your
ROM; share only the zips from the Releases page.*
