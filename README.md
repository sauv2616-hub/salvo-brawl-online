# Salvo Brawl Online

The online version of [Salvo Brawl](https://github.com/sauv2616-hub/salvo-brawl): the same 2–8 player tank brawler, but every player can be on their own computer, in different places, each with their own screen. One computer **hosts** the game and gets a 4-letter room code. Everyone else opens the game, presses **JOIN** and types the code. Guests play with their keyboard, or link their own phone as the controller.

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

1. Open the address and click **HOST A GAME**. The lobby shows a big room code, plus an invite link with a **COPY LINK** button.
2. Send the code (or the link) to your friends.
3. Pick the arena and match settings as usual. You can also add CPU players, and people in the room with you can join on this computer with the keyboard, a game controller, or a phone (scan the QR code).
4. Start the match with **START BRAWL**, or it starts by itself when everyone is ready.

The host's screen works like the local game's big screen. To make it follow your own tank instead of showing the whole battle, press **V** during a match.

**Everyone else**

1. Open the address, type the room code under **JOIN A GAME** and click **JOIN** (or just open the invite link).
2. In the lobby, change your tank with **A / D** (or the ◀ ▶ buttons) and press **G** or **Enter** (or **READY UP**) when you're ready.
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
| Switch weapon | R | U |
| Air strike (when you have one) | E to aim, W A S D move the target, G or E to launch | O |
| Camera: your tank or the whole battle | V | |
| Menu (volume, camera, leave) | Esc | |
| Mute | M | |

### Your phone as your controller (guests)

Once you're in a room, the right side of your lobby shows a QR code and a code of its own. Scan it with your phone and the phone becomes your controller, with the same touch controls as the local version (see *Phone controls*). The phone talks to your computer, and your computer passes everything on to the host. Your keyboard keeps working too.

### Leaving and dropping out

**LEAVE ROOM** (in the lobby or the Esc menu) takes you out. If your connection drops, the game reconnects by itself and you get your spot back. If it can't reconnect within about 40 seconds, it goes back to the start screen. If the host closes their game, the room ends for everyone.

### CPU players

Click **+ ADD CPU** in the lobby (in the open-slot card) to add a computer-controlled tank, up to 5 of them. Each CPU card has **− / +** to set its level from 1 (slow, wild shots, falls off a lot) to 10 (quick, accurate, recovers well, switches weapons by range, grabs power-ups and dodges). Click a CPU's tank name to change its tank, and **×** to remove it. CPUs are always ready, so the brawl starts as soon as every human is ready; it never starts with CPUs alone. The host phone can also add or remove CPUs and set their level.

### Match settings (lobby buttons)

- **MODE · LIVES / MODE · TIMED:** a set number of lives each, last one standing wins; or a timed match. The **− / +** buttons next to it set the lives (1 to 9) or the minutes (1 to 10). In a timed match you respawn every time, score **+1 for every tank you knock out and −1 each time you go down** (including falling off), and the highest score when time runs out wins. If it's tied, the tied players go into **sudden death**: low health, and the next knockout wins.
- **FREE-FOR-ALL / TEAMS:** with TEAMS on, each player is on the red, blue, green or gold team, and everyone on a team drives that colour. Teams can be any size (1 against 3 is fine). New players join the smaller of red and blue; click the team badge on a player's card to move them, or players can tap **TEAM · SWITCH** on their phone. **AUTO TEAMS** splits everyone evenly between red and blue. Teammates can't hurt each other.
- **POWER-UPS:** how often power-ups fall: OFF, LOW, NORMAL, HIGH or CHAOS. Click it to step through. The buttons next to it switch each kind on or off (at least one stays on). See *Power-ups*.
- **MUSIC** and **EFFECTS** sliders: volume for the background music and the sound effects. They're also on the pause screen, and M mutes everything.

### Host phone (phones at the host computer)

The first phone to join is the host (its slot card on the host’s screen says HOST). Once everyone has joined, nobody needs to touch the computer:

- **In the lobby**, the host's phone shows a match setup panel above the tank list: arrows to pick the arena, the mode, lives or minutes, teams and how often power-ups fall. **START MATCH** starts right away, even if not everyone has tapped ready.
- **During a match**, the host has a **MENU** button in the top-right corner. It pauses the game and offers **RESUME** or **END MATCH · MAIN MENU**.
- **After a match**, the host gets **REMATCH** and **MAIN MENU** buttons.

If the host leaves or drops out, the next phone in line becomes the host. The power-up kinds and the volume can only be changed on the computer.

### Full screen on phones

Full screen hides the browser bars and stops the page from zooming when thumbs bump the screen.

- **Android:** tap **FULL SCREEN** on the join screen or in the lobby, or the **⤢** button in the corner of the controller. The phone goes full screen and locks sideways.
- **iPhone:** Safari doesn't let web pages go full screen, so add the controller to the home screen once: tap the **Share** button, choose **Add to Home Screen**, then **Add**. From then on, open **Salvo Pad** from the home screen and type the room code. It runs with no browser bars and can't zoom. The FULL SCREEN button shows these steps too.

Even without full screen, the controller blocks pinch and double-tap zoom while you're playing.

### Phone controls

- **Left half:** put your thumb down anywhere and slide. Left and right drive. **Push up to fire the jetpack.** Pull down to drop through a floating ledge.
- **Right half:** drag in the direction you want to shoot. The farther you drag, the more power. **Let go to fire.** A quick tap fires your last shot again.
- **BOMB button** (bottom right, unlimited bombs): put your thumb on it and drag, just like aiming a missile. The farther you drag, the harder you throw, and the host’s screen shows where the bomb will land. **Let go to throw.** A quick tap without dragging drops a mine under your tank.
- **Weapon button** (above BOMB): tap to switch between missile, machine gun, sniper and bazooka (see *Weapons*). It shows the one you have.
- **AIR STRIKE button** (next to BOMB): appears when you grab an air strike. Tap it, then steer the big red target on the TV with the left stick and tap **LAUNCH**.
- **SOUND** (lobby): your phone plays its own sounds when your tank gets hit, knocks someone out, grabs a power-up or goes down. iPhones stay silent when the ring/silent switch is set to silent.

### Keyboard controls (people at the host computer)

| | Keys 1 | Keys 2 |
|---|---|---|
| Join in the lobby / ready up | G | K |
| Change tank in the lobby | F / H | J / L |
| Drive | A / D | ← / → |
| Jetpack (hold) | W | ↑ |
| Drop through ledge | S | ↓ |
| Aim barrel | F / H | J / L |
| Fire | Hold G to charge, release | Hold K to charge, release |
| Bomb | Hold T to charge, release to throw | Hold I to charge, release to throw |
| Switch weapon | R | U |
| Air strike (when you have one) | E to aim, W A S D move the target, G or E to launch | O to aim, arrows move the target, K or O to launch |

Bombs fly the way your barrel points, so aim with the barrel keys while you hold the bomb key. A quick tap of the bomb key drops a mine. With the machine gun, hold the fire key to keep firing. Esc pauses, M mutes.

Game controllers join with A. Left stick drives (A or LB for jetpack), right stick aims and sets power, RT or RB fires (hold it with the machine gun). B throws bombs: hold the right stick in the direction you want and hold B, then let go of B to throw, or tap B with the stick centred for a mine. Y switches weapon. X calls an air strike: move the target with the left stick, then press X or RT to launch.

### Rules

- Everyone has the same number of lives, **3** unless you change it (or unlimited respawns in a timed match).
- Missiles and bombs drain health. A **direct hit** does the most damage; near misses do less the farther away they land.
- Every hit **knocks you back**, and the less health you have, the farther you fly. Each player's card shows a **knockback multiplier**: ×1.0 at full health, about ×2.2 at half and nearly ×4 when you're almost out. It turns red at ×2 or more.
- Your **jetpack** has about 3.5 seconds of fuel and **refills the moment you land**. Use it to reach higher levels and to fly back after a big knockback.
- Falling off the map is **instant death**: you lose a life no matter how much health you had.
- Running out of health also costs a life. You respawn at the top after a couple of seconds, briefly invincible.
- The camera only zooms in and slows down for the **final knockout** of a match.

### Music

The lobby plays a calm groove. Matches switch to a much harder, faster battle track. In a timed match it speeds up through the last minute, a clock ticks through the last ten seconds, and sudden death runs flat out. In a lives match it picks up for the final showdown, once every tank still in the fight is on its last life.

### Weapons

Every tank carries all four and can switch at any time (a short pause after switching stops quick-swap combos). The tank stats still apply on top.

| Weapon | How it fires | Damage | Reload |
|---|---|---|---|
| ◆ Missile | Arcs; drag farther (or charge longer) for more power | 22 direct, splash around the blast | About 1 second |
| ≡ Machine gun | A stream of fast rounds while you hold the aim; just point it | 3 per round, no splash; each round pushes a little | About 8 rounds a second |
| ⊕ Sniper | A very fast, almost straight shot | 40 direct, small blast | About 2.6 seconds |
| ⬤ Bazooka | A slow, heavy rocket with a high arc | 30 direct and a huge blast radius with big knockback | About 3.2 seconds |

Your card on the host’s screen shows which weapon you have.

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

Pick one of three styles, then its size, or one of the three special arenas.

| Style | Regular | Big (double size) | Mega (for up to 8 players) |
|---|---|---|---|
| Skyforge (sunset sky islands) | Skyforge Isles | Skyforge Archipelago | Skyforge Expanse: a huge island chain, six tiers high |
| Magma (molten decks) | Magma Foundry | Magma Refinery | Magma Inferno: decks and catwalks over a lava sea |
| Frostpeak (ice cliffs) | Frostpeak Basin | Glacier Fortress | Frostfall Citadel: deep valleys and towering cliffs |

| Special arena | Notes |
|---|---|
| Titan Orbital | A space station with five tiers and two wide gaps |
| Warp Nexus | Four portals spread across the station in two linked pairs: the cyan pair joins the bottom-left corner to the upper-right deck, the pink pair joins the bottom-right corner to the upper-left deck. Missiles and thrown bombs go through too. The camera holds still and shows the whole station, so teleports don't make it zoom |
| Rebound Skies | A glowing energy net stretches under the islands. Fall into it and it throws you back up with a full jetpack, but every bounce costs 12 health (and can knock you out if you're low). Fly off the sides past the net and you still fall. Bombs and missiles explode on the net |

Mega maps are wide, so with everyone spread out the camera pulls back a long way and tanks look small. They play best on a big TV.

### Tanks

In the lobby, each player's tank turns on a lit platform in their slot card. Each tank has its own look, but every tank is the same size and uses the same missiles, bombs and jetpack. They differ in these stats:

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

