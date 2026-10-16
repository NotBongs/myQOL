<div align="center">

# ✦ myQOL Client

**One mod, one menu, everything you need.**
A clean, modular quality-of-life client for Fabric, with HUD, visuals, utilities and automation in a single sleek menu.

![Minecraft](https://img.shields.io/badge/Minecraft-26.3-62B47A?style=flat-square)
![Loader](https://img.shields.io/badge/Loader-Fabric-DBB68F?style=flat-square)
![Release](https://img.shields.io/github/v/release/NotBongs/myQOL?style=flat-square&label=Latest&color=FFB000)
![Downloads](https://img.shields.io/github/downloads/NotBongs/myQOL/total?style=flat-square&color=555)

[**Download the latest release**](https://github.com/NotBongs/myQOL/releases/latest)

</div>

---

## Getting started

1. Install [Fabric Loader](https://fabricmc.net/use/installer/) for **Minecraft 26.3**.
2. Download **[Fabric API](https://modrinth.com/mod/fabric-api)** and put it in your `mods` folder.
3. Download `myqol-client-<version>.jar` from [Releases](https://github.com/NotBongs/myQOL/releases/latest) and put it in your `mods` folder.
4. Launch the game and press **Right Shift** to open the menu.

Everything else myQOL needs is already inside the jar, so you don't install anything extra. Sodium, Iris, Lithium, FerriteCore and the other performance mods listed below are included too, so you don't need your own copies.

---

## Features

### HUD
Drag, scale and hide every element in **Edit HUD**.
- **Minimap & World Map**: a minimap and a full world map that remember everywhere you've been
  - Cave mode like Xaero's: **Layered** (a slice below a Top Y you pick with a slider, or auto from the ceiling above you) or **Full** (the first caves under the surface), saved per layer, so caves and the Nether stay mapped
  - Other players with their names and Y level, even through blocks, and a mob radar
  - Biome and block under your mouse, chunk grid, and coordinates, biome, facing, time and light level under the minimap
- **Armor HUD**: armor and held items with durability
- **Inventory HUD**, **Effects HUD**, **Keystrokes**
- **FPS**, **Ping**, **Coordinates**, **Speed**, **Clock**, **Session Timer**
- **Pickup Notifier**: see what you pick up and lose
- **AFK HUD**: timer and status while you're AFK

### Performance & shaders
- **Sodium, Lithium and FerriteCore** built in for much higher FPS and lower memory use
- **Shaders**: Iris built in, with a one-click on/off and shader pack picker
- **More performance**: ImmediatelyFast, ModernFix, Ixeris, Dynamic FPS (lowers FPS when the game is in the background), C2ME (faster chunk loading in singleplayer) and Clumps (merges XP orbs)
- **Resourcify**: browse and install resource packs from inside the game
- **OptiGUI**: custom inventory and container textures from resource packs
- **e4mc**: open your singleplayer world to friends over the internet, no port forwarding
- **Chat Heads**: player heads next to their messages in chat
- **Freecam**: fly the camera around freely (some servers don't allow it, check their rules)
- **ShulkerBoxTooltip**: see what's inside shulker boxes by hovering them
- **Fadeless**: tooltips and the held-item name don't fade out

### Visuals
- **Zoom**: smooth zoom with scroll steps, transitions and spyglass options
- **Crosshair**: dynamic crosshairs, custom colors, and a built-in editor to draw your own
- **Hitboxes**: customizable hitboxes with target and hurt colors
- **Fullbright**: see in the dark

### myQOL Chat
Talk to other myQOL players from any server, Realm or singleplayer world.
- Open chat and press **Tab** with nothing typed, or click the **Chat: Server / ✦ myQOL** button above the chat box, to switch chats
- myQOL messages show in your normal chat with a **[QOL]** tag in your theme color, and each player's ✦ in their badge color
- In myQOL chat: `/msg <player> <message>`, `/r <message>`, `/online`, `/block`, `/unblock`, `/blocked`, `/report <player> [reason]`, `/help`. Any other slash command still goes to the server
- Swear filter (on by default) and join & leave messages under **Utility → myQOL Chat**
- Nobody can chat as someone else: every account is checked with its Mojang-signed chat key

### Account
- **Client Badge**: a ✦ next to players who also use myQOL, in the color each player picks
- **Capes**: capes from OptiFine, MinecraftCapes, LabyMod and more, with a **live 3D preview** you can turn, and a cape/elytra switch

### Utility
- **Waypoints**: folders, icons, block markers and in-world labels
- **Free Look**: look around without turning
- **Elytra Swap**: swap between elytra and chestplate with one key

### Automation
- **Toggle Sprint**, **Auto Eat**, **Auto Tool**, **Anti-AFK**

### The menu
- **Home** page with your own quick toggles, a profile switcher and what's new
- **Profiles**: save complete setups and switch between them in one click
- **Themes**: accent color, blur, transparency and roundness
- **Keybinds** with conflict detection
- **Favorites** and search across every mod

---

## Updating

myQOL checks this page for new versions when the game starts, at most every 6 hours. When there's an update, you'll see a notice and a banner on **Home** with three buttons:

- **Install** downloads the new version and finishes installing when you close Minecraft
- **Ignore** skips that version
- **Details** shows what's new

Nothing is downloaded unless you click **Install**. Your settings, profiles, waypoints and HUD layout are always kept.
You can turn update checks off in **Settings → Updates**.

---

## Privacy

myQOL only connects to these places:

| What | Where | What's sent | Turn it off |
|---|---|---|---|
| Update check | GitHub (`api.github.com`) | Nothing about you, it only reads the latest release | Settings → Updates → Off |
| Client Badges | myQOL presence server | Your Minecraft UUID and star color, and the UUIDs in your player list, about every 2 minutes | Account → Client Badge: turn off **Show Mine To Others**, or switch the badge off |
| myQOL Chat | myQOL server | Your Minecraft name and UUID, the public half of your Minecraft chat key, and the messages you send in myQOL chat | Utility → myQOL Chat: switch it off |

Two bundled mods also go online, only when you use them: **Resourcify** talks to Modrinth/CurseForge while you browse resource packs, and **e4mc** connects to its relay when you open a world to friends.

The presence server only remembers that a UUID was online and its star color, and forgets it after 5 minutes. It stores no names, IPs or servers.

**myQOL Chat** confirms who you are with your Minecraft chat key, the one Mojang gives every account for signed chat: the game signs a one-time code with it, and the chat server checks that Mojang signed your key. Only the public half of the key is sent; your login and private key never leave your PC. Messages are kept for 24 hours so reports can be checked, then deleted. No IPs or servers are stored. Chat stays off if chat is turned off in your Minecraft settings or on your account.

---

## FAQ

<details>
<summary><b>The menu doesn't open</b></summary>

Another mod may be using Right Shift. Change the key in **Settings → General → Open Menu Key**, or in Minecraft's own Controls menu.
</details>

<details>
<summary><b>I don't see stars next to anyone</b></summary>

The ✦ only shows for players who also run myQOL with **Show Mine To Others** on. Check **Account → Client Badge** in the menu. It should say "Connected".
</details>

<details>
<summary><b>myQOL Chat says it couldn't confirm my account</b></summary>

myQOL Chat needs a normal Microsoft/Mojang account with chat allowed. It won't work on offline/cracked accounts, if chat is set to Hidden in your Minecraft settings, or on accounts where chat is turned off. Restarting the game gets you a fresh chat key from Mojang.
</details>

<details>
<summary><b>Does it work on servers and Realms?</b></summary>

Yes. Everything runs on your side, so it works in singleplayer, on servers and on Realms. Always follow the rules of the server you play on.
</details>

<details>
<summary><b>Install says it can't update</b></summary>

Download the jar from [Releases](https://github.com/NotBongs/myQOL/releases/latest), delete the old `myqol-client` jar from your `mods` folder, and put the new one in.
</details>

---

## Bug reports & ideas

Open an [issue](https://github.com/NotBongs/myQOL/issues) and include:
- your myQOL version (shown on **Home**)
- what happened and what you expected
- your `latest.log` from `.minecraft/logs` if the game crashed

---

## Credits

myQOL Client is made by **Bongsy**.

It includes these mods, unmodified, under their own licenses. Their license files are inside the jar.

| Mod | Author | License |
|---|---|---|
| [Zoomify](https://github.com/isXander/Zoomify) | isXander | LGPL-3.0 |
| [YetAnotherConfigLib](https://github.com/isXander/YetAnotherConfigLib) | isXander | LGPL-3.0 |
| [Dynamic Crosshair](https://github.com/Crendgrim/DynamicCrosshair) | Crendgrim | LGPL-3.0 |
| [Cape Provider](https://github.com/litetex-oss/mcm-cape-provider) | litetex | LGPL-2.1 |
| [Sodium](https://github.com/CaffeineMC/sodium) | JellySquid / CaffeineMC | PolyForm Shield 1.0.0 |
| [Lithium](https://github.com/CaffeineMC/lithium-fabric) | JellySquid, 2No2Name | LGPL-3.0 |
| [FerriteCore](https://github.com/malte0811/FerriteCore) | malte0811 | MIT |
| [Iris](https://github.com/IrisShaders/Iris) | coderbot, IMS212 and contributors | LGPL-3.0 |
| [ImmediatelyFast](https://github.com/RaphiMC/ImmediatelyFast) | RK_01 | LGPL-3.0 |
| [ModernFix](https://github.com/embeddedt/ModernFix) | embeddedt | LGPL-3.0 |
| [Ixeris](https://github.com/decce6/Ixeris) | decce | LGPL-3.0 |
| [Dynamic FPS](https://github.com/juliand665/Dynamic-FPS) | juliand665, LostLuma | MIT |
| [C2ME](https://github.com/RelativityMC/C2ME-fabric) | RelativityMC, ishland | MIT |
| [Clumps](https://github.com/jaredlll08/Clumps) | Jaredlll08 | MIT |
| [Resourcify](https://github.com/DeDiamondPro/Resourcify) | DeDiamondPro | LGPL-3.0 |
| [OptiGUI](https://github.com/opekope2/OptiGUI) | opekope2 | MIT |
| [e4mc](https://github.com/vgskye/e4mc-minecraft-architectury) | skyevg | MIT |
| [Chat Heads](https://github.com/dzwdz/chat_heads) | dzwdz, Fourmisain | MPL-2.0 |
| [Freecam](https://github.com/MinecraftFreecam/Freecam) | hashalite, Matt Sturgeon | MIT |
| [ShulkerBoxTooltip](https://github.com/MisterPeModder/ShulkerBoxTooltip) | MisterPeModder | MIT |
| [Fadeless](https://github.com/DerpDerpling/Fadeless) | DerpDerpling, UltimateBoomer | MIT |
| [Fabric Language Kotlin](https://github.com/FabricMC/fabric-language-kotlin) | FabricMC | Apache-2.0 |

Menu icons are from [Phosphor Icons](https://phosphoricons.com) (MIT).

<div align="center">

**Not affiliated with Mojang or Microsoft.**

</div>
