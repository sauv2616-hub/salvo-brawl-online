# Salvo Online

The online version of [Salvo](https://github.com/sauv2616-hub/salvo-brawl): the same 2–8 player tank brawler, but every player can be on their own computer, in different places, each with their own screen. One computer **hosts** the game and gets a 4-letter room code. Everyone else opens the game, presses **JOIN** and types the code. Guests play with their keyboard, or link their own phone as the controller.

It is a separate copy of the game. The local version in the `salvo-brawl` repository is untouched and keeps working as before.

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The game. Everyone opens this: the host clicks **HOST A GAME**, everyone else **JOIN A GAME**. |
| `controller.html` | The phone controller. Phones open it by scanning a QR code. |
| `manifest.webmanifest` | Lets phones add the controller to their home screen and run it full screen. |
| `icon-192.png`, `icon-512.png` | The controller's home-screen icon. |
| `README.md` | This guide. |

## Turn on the website (one time, about 2 minutes)

No game server or add-on is needed. GitHub Pages hosts the files, and the computers connect to each other directly (see *How it works*).

1. Open the repository on GitHub: `github.com/sauv2616-hub/salvo-brawl-online`.
2. Click the **Settings** tab, then **Pages** in the left sidebar.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Pick the **main** branch and the **/ (root)** folder, then click **Save**.
4. Wait a minute or two and refresh the page. It shows the address: **https://sauv2616-hub.github.io/salvo-brawl-online/**

Everyone uses that same address.

## Playing online

**The host**

The host should be the player with the best internet connection: the match runs on their computer and their tab needs to stay open. It keeps running if they switch to another tab or window; just don't close it.

1. Open the address and click **HOST A GAME**. The lobby shows a big room code, plus an invite link with a **Copy link** button. The leave icon at the top right closes the room.
2. Send the code (or the link) to your friends.
3. Pick the arena and match settings as usual. You can also add CPU players, and people in the room with you can join on this computer with the keyboard, a game controller, or a phone (scan the QR code).
4. Start the match with **Start match**, or it starts by itself when everyone is ready.

The host's screen works like the local game's big screen. To make it follow your own tank instead of showing the whole battle, press **V** during a match.

**Everyone else**

1. Open the address, type the room code under **JOIN A GAME** and click **JOIN** (or just open the invite link).
2. Your lobby looks like the host's: the arena and settings on the left (the host picks those), everyone's tanks in the middle, and the CPUs on the right. Change your tank with **A / D** (or click your tank's name), change your two weapons with **R** (or click them), and press **G** or **Enter** (or **Ready up**) when you're ready.
3. During a match your screen follows your own tank and anyone near it. Press **V** to switch to the whole battle and back.

Guests can't change the arena or settings; the host picks those. If a match is already running when you join, you watch it and join the next one.

Guests need a keyboard, so join from a computer. A phone can't be a full guest on its own, but it can be a guest's controller (see below).

### Guest keys

| | Keys | Also works |
|---|---|---|
| Drive | A / D | ← / → |
| Jetpack (hold) | W | ↑ |
| Drop through ledge | S | ↓ |
| Aim barrel | F / H | J / L |
| Fire | Hold G to charge, release (machine gun: hold) | K |
| Bomb | Hold T to throw along the barrel, tap for a mine | I |
| Swap between your two weapons (in the lobby: change which two) | R | U |
| Air strike (when you have one) | E to aim, W A S D move the target, G or E to launch | O |
| Camera: your tank or the whole battle | V | |
| Menu (volume, camera, leave) | Esc | |
| Mute | M | |

### Change any key, or aim with the mouse

Guests can change every key too: open settings (the gear in your lobby) or **KEYS** in the Esc menu, click **Customize keys**, click a key and press the new one. Your keys are saved on your computer.

**Mouse aims** in the same settings is on to start with: point to aim (the farther from your tank, the more power), click to fire (hold to see the shot first; hold with the machine gun to keep firing), right-click (two-finger click on a trackpad) for a mine or hold it to throw a bomb, and during an air strike the target follows the pointer. Your keys keep working alongside it.

### Your phone as your controller (guests)

Once you're in a room, the right side of your lobby shows a QR code and a code of its own. Scan it with your phone and the phone becomes your controller, with the same touch controls as the local version (see *Phone controls*). The phone talks to your computer, and your computer passes everything on to the host. Your keyboard keeps working too.

### Leaving and dropping out

The leave icon (top right of your lobby) or **LEAVE ROOM** in the Esc menu takes you out. If your connection drops, the game reconnects by itself and you get your spot back. If it can't reconnect within about 40 seconds, it goes back to the start screen. If the host closes their game, the room ends for everyone.

### The lobby

- **Left:** the match setup. Pick one of the six arena types, its size (**Small**, **Big** or **Mega**) and the map type (**Regular**, **Bounce** or **Active**), then the match rules underneath. The arena you pick is shown live behind the lobby.
- **Middle:** every player's tank, big, turning slowly on a show platform with its driver standing beside it. The driver waves once that player is ready. Under each tank is the player's name plate: their tank, their two weapons and how they're playing (keys, controller or phone). Keyboard and controller players can click their tank's name or weapons to change them. Click the team badge to move a player to another team, and **×** to remove them.
- **Right:** the room code and QR code for phones, the CPU players, and **Start match**.
- **Top right:** three icons. The gear opens the sound settings (music and effects volume), the keyboard opens the controls, and the last one goes full screen.

### CPU players

Click **+ Add CPU** in the CPUs panel on the right to add a computer-controlled tank, up to 5 of them. Each CPU gets a small row instead of a big turntable. Use **− / +** to set its level from 1 (slow, wild shots, falls off a lot) to 10 (quick, accurate, recovers well, switches weapons by range, grabs power-ups and dodges). Click its tank name to change its tank, its weapons to change its two weapons, and **×** to remove it. CPUs are always ready, so the brawl starts as soon as every human is ready; it never starts with CPUs alone. The host phone can also add or remove CPUs and set their difficulty.

### Match settings

- **Mode · Lives / Timed:** a set number of lives each, last one standing wins; or a timed match. The **− / +** buttons set the lives (1 to 9) or the minutes (1 to 10). In a timed match you respawn every time, score **+1 for every tank you knock out and −1 each time you go down** (including falling off), and the highest score when time runs out wins. If it's tied, the tied players go into **sudden death**: low health, and the next knockout wins.
- **Teams · Free-for-all / Teams:** with Teams on, each player is on the red, blue, green or gold team, and everyone on a team drives that colour. Teams can be any size (1 against 3 is fine). New players join the smaller of red and blue; click the team badge on a player's card to move them, or players can tap **TEAM · SWITCH** on their phone. **Auto** splits everyone evenly between red and blue. Teammates can't hurt each other. When two or more real players (not CPUs) are on the same team, each one gets a coloured dot and their tag in their own player colour (on their card, above their tank and on the phone), so teammates can tell each other apart while their tanks stay the team colour.
- **Power-ups:** click it to open a small panel: how often power-ups fall (Off, Low, Normal, High or Chaos) and which kinds can drop (at least one stays on). See *Power-ups*.
- **Sound:** the gear icon at the top right has the music and effects volume. They're also on the pause screen, and M mutes everything.

### Host phone (phones at the host computer)

The first phone to join is the host (its name plate says HOST). Once everyone has joined, nobody needs to touch the computer. The host's phone has two tabs so it never gets crowded:

- **1 · Your tank:** pick your two weapons and your tank, like every other phone. **Next · Match setup** at the bottom takes you to the second tab.
- **2 · Match setup:** the arena type, the arena size, the map type (Regular, Bounce or Active), how often power-ups drop and which kinds, how many bots and how hard they are, lives or timed, and teams.
- **Start match** starts right away, even if not everyone has tapped ready.
- **During a match**, the host has a **MENU** button in the top-right corner. It pauses the game and offers **RESUME** or **END MATCH · MAIN MENU**.
- **After a match**, the host gets **REMATCH** and **MAIN MENU** buttons.

If the host leaves or drops out, the next phone in line becomes the host. The volume can only be changed on the computer.

### Full screen on phones

Full screen hides the browser bars and stops the page from zooming when thumbs bump the screen.

- **Android:** tap **FULL SCREEN** on the join screen or in the lobby, or the **⤢** button in the corner of the controller. The phone goes full screen and locks sideways.
- **iPhone:** Safari doesn't let web pages go full screen, so add the controller to the home screen once: tap the **Share** button, choose **Add to Home Screen**, then **Add**. From then on, open **Salvo Pad** from the home screen and type the room code. It runs with no browser bars and can't zoom. The FULL SCREEN button shows these steps too.

Even without full screen, the controller blocks pinch and double-tap zoom while you're playing.

### Phone controls

- **Left half:** put your thumb down anywhere and slide. Left and right drive. **Push up to fire the jetpack.** Pull down to drop through a floating ledge.
- **Right half:** drag in the direction you want to shoot. The farther you drag, the more power. **Let go to fire.** A quick tap fires your last shot again.
- **BOMB button** (bottom right, unlimited bombs): put your thumb on it and drag, just like aiming a missile. The farther you drag, the harder you throw, and the host’s screen shows where the bomb will land. **Let go to throw.** A quick tap without dragging drops a mine under your tank.
- **Weapon button** (above BOMB): tap to swap between your two weapons (see *Weapons*). It shows the one you have.
- **AIR STRIKE button** (next to BOMB): appears when you grab an air strike. Tap it, then steer the big red target on the TV with the left stick and tap **LAUNCH**.
- **SOUND** (lobby): your phone plays its own sounds when your tank gets hit, knocks someone out, grabs a power-up or goes down. iPhones stay silent when the ring/silent switch is set to silent.

### Keyboard controls (people at the host computer)

| | Keys 1 | Keys 2 |
|---|---|---|
| Join in the lobby / ready up (the fire key) | G | K |
| Change tank in the lobby | F / H | J / L |
| Drive | A / D | ← / → |
| Jetpack (hold) | W | ↑ |
| Drop through ledge | S | ↓ |
| Aim barrel | F / H | J / L |
| Fire | Hold G to charge, release | Hold K to charge, release |
| Bomb | Hold T to charge, release to throw | Hold I to charge, release to throw |
| Swap between your two weapons (in the lobby: change which two) | R | U |
| Air strike (when you have one) | E to aim, W A S D move the target, G or E to launch | O to aim, arrows move the target, K or O to launch |

Bombs fly the way your barrel points, so aim with the barrel keys while you hold the bomb key. A quick tap of the bomb key drops a mine. With the machine gun, hold the fire key to keep firing. Esc pauses, M mutes.

### Change any key

Every keyboard key can be changed. Open settings (the gear at the top right of the lobby, or **KEYS** on the pause screen) and click **Customize keys**. Click the key you want to change, then press the new one. If another action already uses that key, the two swap, so nothing ends up on two jobs. Esc cancels, and **Reset to default** puts everything back. Your keys are saved on this computer, and the lobby hints and the controls list (the keyboard icon) always show the keys you picked. Esc (pause), M (mute) and Enter (start) can't be used.

### Mouse or trackpad aiming

One keyboard player can aim with the mouse or trackpad. It's Keys 1 to start with; change it (Keys 1, Keys 2 or Off) under **Mouse aims** in settings or in the Customize keys window.

- **Point** to aim: the barrel follows the pointer. The farther the pointer is from your tank, the more power.
- **Click** to fire. Hold the click to see where the shot will go, then let go to fire. With the machine gun, hold the click to keep firing.
- **Right-click** (a two-finger click on most trackpads) drops a mine. Hold the right button to throw a bomb toward the pointer instead. The bomb key still throws along the barrel too.
- **Air strike:** the big target follows the pointer; click to launch.

The keyboard keys keep working alongside the mouse, and the pointer turns into a crosshair during a match.

### Game controllers

Game controllers join with A. Left stick drives (A or LB for jetpack), right stick aims and sets power, RT or RB fires (hold it with the machine gun). B throws bombs: hold the right stick in the direction you want and hold B, then let go of B to throw, or tap B with the stick centred for a mine. Y swaps between your two weapons (in the lobby it changes which two). X calls an air strike: move the target with the left stick, then press X or RT to launch.

### Rules

- Everyone has the same number of lives, **3** unless you change it (or unlimited respawns in a timed match).
- Missiles and bombs drain health. A **direct hit** does the most damage; near misses do less the farther away they land.
- Every hit **knocks you back**, and the less health you have, the farther you fly. Each player's card shows a **knockback multiplier**: ×1.0 at full health, about ×2.2 at half and nearly ×4 when you're almost out. It turns red at ×2 or more.
- Your **jetpack** has about 3.5 seconds of fuel and **refills the moment you land**. Use it to reach higher levels and to fly back after a big knockback.
- Falling off the map is **instant death**: you lose a life no matter how much health you had.
- Running out of health also costs a life. You respawn at the top after a couple of seconds, briefly invincible.
- The camera only zooms in and slows down for the **final knockout** of a match. The screen shakes when tanks get hit, and shakes less the more tanks there are, so an 8-player brawl stays easy to watch.

### Music

The lobby plays a calm groove. Matches switch to a pumping battle track built in four-bar phrases: the drums and a rolling bass start it off, then a sweeping arpeggio comes in, then the lead riff, then everything at once with a snare-roll build, and each new phrase lands with a crash and a deep drop. In a timed match it speeds up through the last minute, a clock ticks through the last ten seconds, and sudden death plays every layer flat out. In a lives match it picks up for the final showdown, once every tank still in the fight is on its last life.

### Weapons

Before each match, every player picks **two of the four weapons** and can only use those two during the match. You can swap between them at any time (a short pause after swapping stops quick-swap combos), and the tank stats still apply on top.

- **Phone:** in the lobby, tap two weapon cards. The one marked **START** is the one you begin the match with; tap your other one to make it the starting weapon instead. In the match, the weapon button swaps between your two.
- **Keyboard:** in the lobby, **R** (Keys 1) or **U** (Keys 2) steps through the possible pairs, or click the weapons on your name plate. In the match, the same key swaps.
- **Game controller:** **Y** steps through the pairs in the lobby and swaps in the match.
- **CPUs** get a random pair; click a CPU's weapons to change them.

| Weapon | How it fires | Damage | Reload |
|---|---|---|---|
| ◆ Missile | Arcs; drag farther (or charge longer) for more power | 22 direct, splash around the blast | About 1 second |
| ≡ Machine gun | A stream of fast rounds while you hold the aim; just point it | 3 per round, no splash; each round pushes a little | About 8 rounds a second |
| ⊕ Sniper | A very fast, almost straight shot | 40 direct, small blast | About 2.6 seconds |
| ⬤ Bazooka | A slow, heavy rocket with a high arc | 30 direct and a huge blast radius with big knockback | About 3.2 seconds |

Your card on the host’s screen shows the weapon you have and the other one you can swap to.

### Bombs

- Bombs **never run out**. After each one there's a short cooldown (about 1 second) before you can use the next. The bomb button on the phone dims while it cools down.
- A bomb does more damage than a missile (up to 30) and has a bigger blast.
- **Thrown bombs** are aimed like missiles (see the controls). They arc, bounce, and explode after about 2.5 seconds, or right away if they hit a tank. You can throw as many as you like.
- **Mines** sit where they land, arm after a moment (the light starts blinking), and go off when an enemy drives over them. They last 20 seconds.
- **Two mines at most:** you can have two mines planted at once. Dropping a third sets off both of the planted ones, wherever they are, and plants the new one. That makes a handy remote trigger: plant two, wait for someone to walk past, then drop another. Throwing bombs never sets your mines off.
- The dots on your phone's bomb button and on your card show how many mines you have planted.
- Your own bombs never hurt you, but their blast still pushes you, so a mine under your own tank works as a rocket jump.
- Shooting a bomb or mine sets it off, and explosions set off any bombs nearby.

### Power-ups (optional)

Pick how often they fall with the **POWER-UPS** button in the lobby: **LOW** (every 24–34 seconds), **NORMAL** (13–20), **HIGH** (6–10) or **CHAOS** (2–4). Only one is on the map at a time; drive into it to grab it. Ones nobody grabs disappear after a while. The buttons next to POWER-UPS turn each kind on or off.

| Power-up | What it does |
|---|---|
| ★ Star | Fire twice as fast for 16 seconds. Your tank glows gold. |
| ⬢ Shield | A bubble blocks all damage and knockback for 16 seconds. It doesn't stop you falling off the map. |
| ⇈ Wings | Wings sprout from your tank and your jetpack never runs out for 16 seconds, so you can fly the whole time without landing. |
| ▾ Tiny | Your tank shrinks to half size for 16 seconds, so missiles and bombs often fly right over it. Knockback stays exactly the same as normal size. |
| ✚ Med kit | +15 health straight away (up to your maximum). |
| ✹ Spam bombs | No bomb cooldown for 16 seconds: throw as fast as you can tap. |
| ☄ Mega missile | Your next shot is a huge missile: 4× damage, a massive blast and extra knockback. Use it within 30 seconds. |
| ➶ Heat seeker | Your next shot is a slow missile that chases the nearest enemy for 8 seconds, then explodes in the air if it hasn't hit anything. Shooting it down works too. Use it within 30 seconds. |
| ◎ Air strike | Kept until you use it (or go down). Calling it shows a giant red target on the host’s screen; steer it, then launch, and three missiles fly in from the screen and blast the area. While you aim, your tank can't move and can still be hit. It launches by itself after 12 seconds. |

### Arenas

There are six arena types, and each one comes in three sizes: **Small**, **Big** (about double) and **Mega** (huge, for up to 8 players). Every type changes the game in its own way.

| Type | Small | Big | Mega | What's special |
|---|---|---|---|---|
| Skyforge (grass) | Skyforge Isles | Skyforge Archipelago | Skyforge Expanse | Classic floating islands. No tricks, just solid ground. |
| Frostpeak (ice) | Frostpeak Basin | Glacier Fortress | Frostfall Citadel | Slippery ice: tanks slide and take a moment to stop or turn round. |
| Magma (fire) | Magma Foundry | Magma Refinery | Magma Inferno | Lava vents in the decks rumble, then erupt every few seconds, launching (and burning) whoever is standing on them. |
| Titan (space) | Titan Outpost | Titan Orbital | Titan Megastation | Low gravity: tanks jump and fall slower, and shells fly in longer, floatier arcs. |
| Warp (portals) | Warp Junction | Warp Nexus | Warp Labyrinth | Linked portals (shown by colour) teleport tanks, missiles and bombs. The camera holds still so teleports don't make it jump. |
| Abyss (underwater) | Coral Reef | Sunken Ruins | Abyssal Trench | Tanks sink slowly, and a current slowly drifts back and forth, pushing tanks and shots with it. |

**Map type** (pick one; the bounce floor and active map can't be on together):

- **Regular:** the arena as it is.
- **Bounce:** a glowing energy net stretches under the arena. Fall into it and it throws you back up with a full jetpack, but every bounce costs 12 health (and can knock you out if you're low). Fly off the sides past the net and you still fall. Bombs and missiles explode on the net.
- **Active:** the map changes while you play. Every 11 to 17 seconds a warning banner comes up and something happens. Half the time a group of platforms (the left side, the right side, the top platforms or the bottom decks) blinks red, crumbles away, and comes back about 6 seconds later, so get off them when they blink. The other half is the arena's own event:

| Type | Active-map event |
|---|---|
| Skyforge | **Wind gust:** a strong wind blows everything one way for a few seconds. |
| Frostpeak | **Avalanche incoming:** a wall of snow sweeps across the high or low half of the map, hitting and shoving every tank in its way. |
| Magma | **Lava is rising:** the lava climbs up over the bottom decks, holds there, then drains. Touching it burns and throws you upward. |
| Titan | **Meteor shower:** meteors rain down and explode where they land. |
| Warp | **Portals haywire:** every portal leads somewhere random for a few seconds. |
| Abyss | **Tidal surge:** a powerful current pushes everything one way. |

CPU players see the warnings too and try to get off dropping platforms and away from rising lava.

Mega maps are wide, so with everyone spread out the camera pulls back a long way and tanks look small. They play best on a big TV.

### Tanks

In the lobby, each player's tank turns slowly on a show platform with its driver standing beside it. Each tank has its own look, but every tank is the same size and uses the same missiles, bombs and jetpack. They differ in these stats (the phone shows them when you pick a tank):

| Tank | Role | Strengths | Trade-offs |
|---|---|---|---|
| Vanguard | All-rounder | Even in every stat | No standout strengths |
| Striker | Scout | 25% faster, 25% more jet fuel, slightly quicker reload | 15% less health, easier to knock back |
| Bulwark | Heavy | 28% more health, 28% harder to knock back, 5% more damage | 20% slower, reloads 22% slower, 15% less jet fuel |
| Ravager | Demolition | 15% bigger blasts, 10% more damage, 20% more knockback | Reloads 10% slower, a little slower to drive |
| Viper | Rapid fire | Reloads 26% faster, faster missiles | 22% less damage, 10% less health, smaller blasts |

## If something goes wrong

- **"No game is open with room code …":** check the code on the host's screen. If the host just opened or reloaded the game, wait a few seconds and try again. Room codes are letters only.
- **"Found room … but couldn't link up":** one of the networks is blocking direct connections. This happens on some school, work and public Wi-Fi. Try a different network; a phone hotspot usually works. The game also tries free public relay servers automatically, but they come with no guarantees.
- **"Couldn't reach the game server":** your internet connection or network is blocking PeerJS's connection server. Check the connection, or try another network.
- **"Room … is full":** 8 players is the limit, including CPUs and local players on the host computer.
- **The game feels slightly behind:** each guest sees the host's game a fraction of a second late (usually about 0.15 seconds), a bit more over long distances or busy Wi-Fi. That is normal for online play. The host's own computer has no delay, so for the fairest games the host can be the player with the strongest connection.
- **A guest's phone won't link:** the phone links to the guest's computer, so it needs to be able to reach that computer (being on the same Wi-Fi is the most reliable). Scan the QR code on the guest's lobby screen, not the host's.
- **The host's screen shows "NO ROOM":** the host computer couldn't reach the connection server. Check the internet connection and click **TRY AGAIN**.

## How it works

GitHub Pages only serves files; it can't run a game server. So one player's computer runs the game (the host), and the other computers connect straight to it using WebRTC, the same peer-to-peer technology video calls use. PeerJS's free public server only introduces the computers to each other; after that, the game traffic goes directly between them. When a network doesn't allow a direct link, the traffic goes through a free public relay instead (PeerJS's or Metered's Open Relay).

The host runs the real match. Twenty times a second it sends every guest where each tank, missile, bomb and power-up is, plus every explosion and sound, and each guest draws the battle itself with its own camera. Guests send their key presses (or their phone's input) back to the host. Nothing is stored online and no accounts are needed. Each guest uses roughly 10–40 KB per second.

**Optional, only if friends often can't link up:** a dedicated relay (a "TURN server") makes connections work on almost any network. Metered.ca has a free plan; it gives you a username and password that would be added to the connection list in `rtcConfig()` in both `index.html` and `controller.html`. This isn't needed for most home networks.

