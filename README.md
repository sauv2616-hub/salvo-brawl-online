# Salvo Online

The online version of [Salvo](https://github.com/sauv2616-hub/salvo-brawl): the same 2–8 player tank brawler, but every player can be on their own computer, in different places, each with their own screen. One computer (or phone) **hosts** the game and gets a 4-letter room code. Everyone else opens the game, presses **JOIN** and types the code. Guests play with their keyboard, or link their own phone as the controller.

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

1. Open the address, type your name under **YOUR NAME** (up to 12 letters; it's saved for next time) and click **HOST A GAME**. The lobby shows a big room code, plus an invite link with a **Copy link** button. The leave icon at the top right closes the room.
2. Send the code (or the link) to your friends.
3. Pick the arena and match settings as usual. You can also add CPU players, and people in the room with you can join on this computer with the keyboard, a game controller, or a phone (scan the QR code).
4. Start the match with **Start match**, or it starts by itself when everyone is ready.

The host's screen works like the local game's big screen. To make it follow your own tank instead of showing the whole battle, press **V** during a match.

**Everyone else**

1. Open the address, type your name under **YOUR NAME**, then the room code under **JOIN A GAME**, and click **JOIN** (or just open the invite link). Your name shows over your tank and on everyone's scoreboard.
2. Your lobby looks like the host's: the arena and settings on the left (the host picks those), everyone's tanks in the middle, and the CPUs on the right. Change your tank with **A / D** (or click your tank's name), change your two weapons with **R** (or click them), and press **G** or **Enter** (or **Ready up**) when you're ready.
3. During a match your screen follows your own tank and anyone near it. Press **V** to switch to the whole battle and back.

Guests can't change the arena or settings; the host picks those. If a match is already running when you join, you watch it and join the next one.

Guests usually join from a computer. A phone can join on its own too (see *No computer? Play on your phone*), or be a guest's controller (see below).

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
| Menu (volume, camera, name tags, leave) | Esc or P | |
| Mute | M | |

### No computer? Play on your phone

Someone with only a phone can still join an online game. Open the game's address on the phone (or tap **NO COMPUTER? PLAY ON THIS PHONE** on the phone controller page), type the room code and tap **JOIN**. The phone shows the game itself, following your tank, with the same touch controls as the phone controller on top: left thumb drives (push up to jet, pull down to drop), right thumb drags to aim and lets go to fire, plus the **BOMB**, weapon-swap and air-strike buttons. **MENU** (top right) has the camera, keys and leave options, and **⤢ FULL** goes full screen. Turn the phone sideways to play. Your thumbs cover part of a small screen, so a computer (or a phone used as a controller next to a computer) is still the better way to play; this is for when there's no computer around.

### Host from your phone

A phone can host a game too. Open the address on the phone, type your name and tap **HOST A GAME**. The phone runs the match itself and you play on it with the same touch controls as above. Send the room code (or the invite link) to everyone else.

On a phone the host lobby is laid out for thumbs: the room code and the CPUs come first, then your tank, then the match settings, with **START MATCH** pinned to the bottom of the screen. During a match, **MENU** pauses it. People on their own computers can press **P** (or Esc, or the **MENU** button at the top left) for their own menu, where they can also change the name tags. The phone tries to keep its screen on while it hosts. Keep the game open in front: phones pause web pages when you switch apps or lock the screen, and that freezes the match for everyone. The hosting phone does all the work for every player, so a recent phone works best, and smaller matches run smoothest.

### Change any key, or aim with the mouse

Guests can change every key too: open settings (the gear in your lobby) or **KEYS** in the Esc menu, click **Customize keys**, click a key and press the new one. Your keys are saved on your computer.

**Mouse aims** in the same settings is on to start with: point to aim (the farther from your tank, the more power), click to fire (hold to see the shot first; hold with the machine gun to keep firing), right-click (two-finger click on a trackpad) for a mine or hold it to throw a bomb, and during an air strike the target follows the pointer. Your keys keep working alongside it.

### Your phone as your controller (guests)

Once you're in a room, the right side of your lobby shows a QR code and a code of its own. Scan it with your phone and the phone becomes your controller, with the same touch controls as the local version (see *Phone controls*). The phone talks to your computer, and your computer passes everything on to the host. Your keyboard keeps working too.

### Leaving and dropping out

The leave icon (top right of your lobby) or **LEAVE ROOM** in the Esc menu takes you out. If your connection drops, the game reconnects by itself and you get your spot back. If it can't reconnect within about 40 seconds, it goes back to the start screen. If the host closes their game, the room ends for everyone.

### The lobby

- **Left:** the match setup. The **arena** drop-down lists the seven arena types with a little map of each; the size buttons under it pick **Small**, **Big** or **Mega**. The **map type** drop-down picks **Regular**, **Classic**, **Bounce**, **Active** or **Rising** (see *Map type*), and the match rules sit underneath. The arena you pick is shown live behind the lobby, a little darker so the tanks stand out.
- **Middle:** every player's tank, big, turning slowly on a plain dark turntable under a spotlight. Under each tank is the player's name plate: their name (or P number), their tank, their two weapons and how they're playing (keys, controller or phone). Keyboard and controller players can click their tank's name or weapons to change them. Click the team badge to move a player to another team, and **×** to remove them.
- **Right:** the room code and QR code for phones, the CPU players, and **Start match**.
- **Top right:** the gear opens the settings: music and effects volume, mouse aiming, and **Customize keys**, which shows and changes every control. The icon next to it goes full screen.

### CPU players

Click **+ Add CPU** in the CPUs panel on the right to add a computer-controlled tank, up to 5 of them. Each CPU gets a small row instead of a big turntable. Use **− / +** to set its level from 1 (slow, wild shots, falls off a lot) to 10 (quick, accurate, recovers well, switches weapons by range, grabs power-ups and dodges). Click its tank name to change its tank, its weapons to change its two weapons, and **×** to remove it. CPUs are always ready, so the brawl starts as soon as every human is ready; it never starts with CPUs alone. A CPU that can't find a clear shot for a few seconds (a wall or a tower in the way) moves in and hops, or jets across the gap, to get a new angle, so matches don't stall.

### Match settings

- **Mode · Lives / Timed / Keep Away:** a set number of lives each, last one standing wins; or a timed match. The **− / +** buttons set the lives (1 to 9) or the minutes (1 to 10). In a timed match you respawn every time, score **+1 for every tank you knock out and −1 each time you go down** (including falling off), and the highest score when time runs out wins. If it's tied, the tied players go into **sudden death**: low health, and the next knockout wins.
- **Mode · Keep Away:** grab the power core and keep it away from everyone else for as long as you can. The core (a white-hot crystal in a spinning cage, glowing through every colour) drops in at the top of the arena; drive into it to grab it, and your clock (on your card) runs for as long as you carry it. Everyone else is out to knock you down and take it. Getting knocked out drops it: it pops out and rolls around until someone else picks it up. If it falls off the map (or into lava or a rising hazard), it comes back at the top. Every attack does **2.5× damage** in this mode but knocks tanks back about 30% less, so tanks go down (and the core changes hands) a lot more often than they fly off. If it touches a bounce net it also comes back at the top. You respawn every time. There's no match clock: the **− / +** buttons set how long you need to hold it (15 seconds to 5 minutes, 1:00 to start with), and the first player (or team, adding up its players' times) to hold it that long wins. The clock at the top shows the leader's time and the goal. CPUs go after the core and its carrier too.
- **Teams · Free-for-all / Teams:** with Teams on, each player is on the red, blue, green or gold team, and everyone on a team drives that colour. Teams can be any size (1 against 3 is fine). New players join the smaller of red and blue; click the team badge on a player's card to move them, or players can tap **TEAM · SWITCH** on their phone. **Auto** splits everyone evenly between red and blue. Teammates can't hurt each other, and in every mode each team starts together on its own side of the map (red on the left, blue on the right, then green and gold in between when there are more teams). In timed and Keep Away games your team also respawns on its own side of the centre. When two or more real players (not CPUs) are on the same team, each one gets a coloured dot and their tag in their own player colour (on their card, above their tank and on the phone), so teammates can tell each other apart while their tanks stay the team colour.
- **Power-ups:** click it to open a small panel: how often power-ups fall (Off, Low, Normal, High or Chaos) and which kinds can drop (at least one stays on). See *Power-ups*.
- **Sound:** the gear icon at the top right has the music and effects volume. They're also on the pause screen, and M mutes everything.
- **Name tags:** the gear also sets the tags over the tanks, so you can find yours without them getting in the way. **Size** goes from Small to Huge. **Style:** *Minimal* shows just the P number and a small marker, *Standard* shows the name with a health and jet bar, and *Bold* puts each name on a plate in its colour, with bigger bars and a brighter glow on the ground under the tank. The same choices are on the pause screen (and in a guest's Esc menu), so you can try them mid-match and see the difference straight away. They're saved on that computer.

### Host phone (phones at the host computer)

The first phone to join is the host (its name plate says HOST). Its lobby is the same as every other phone's (see *Your phone in the lobby*), so it stays simple; the arena and match settings are picked on the big screen.

- **START** (next to READY UP) starts the match right away, even if not everyone has tapped ready.
- **During a match**, the host has a **MENU** button in the top-right corner. It pauses the game and offers **RESUME** or **END MATCH · MAIN MENU**.
- **After a match**, the host gets **REMATCH** and **MAIN MENU** buttons.

If the host leaves or drops out, the next phone in line becomes the host. The volume can only be changed on the computer.

### Full screen on phones

Full screen hides the browser bars and stops the page from zooming when thumbs bump the screen.

- **Android:** tap **FULL SCREEN** on the join screen or in the lobby, or the **⤢** button in the corner of the controller. The phone goes full screen and locks sideways.
- **iPhone:** Safari doesn't let web pages go full screen, so add the controller to the home screen once: tap the **Share** button, choose **Add to Home Screen**, then **Add**. From then on, open **Salvo Pad** from the home screen and type the room code. It runs with no browser bars and can't zoom. The FULL SCREEN button shows these steps too.

Even without full screen, the controller blocks pinch and double-tap zoom while you're playing.

### Your phone in the lobby

- **Your name:** type it under **YOUR NAME** on the join screen (up to 12 letters). If you join straight from the QR code, the phone asks for it once. Your name goes over your tank, on your card, on the scoreboard and on the winner screen; players without a name show their P number. The phone shows your name big at the top, with your P number next to it.
- **Menu:** the **⋯** button at the top right opens the menu: change your name, turn the phone's own sound on or off, go full screen, or leave the game.
- **Your tank:** it turns on a stage in your colour, with its name and role underneath. Swipe it left or right (or tap the arrows) for the next one. The yellow **?** button in its corner opens the tank's stats card: speed, armour, blast, reload and jet bars, what makes it different and the two weapons you've picked. Tap **?** again (or the card) to close it; it updates as you change tanks, so you can compare them.
- **Loadout reels:** under the stage (beside it when the phone is sideways) are three reels, a bit like a kart picker: **TANK**, **WEAPON 1** and **WEAPON 2**. Drag a reel up or down, tap the item above or below the yellow frame, or use the **▲ / ▼** arrows. Weapon 1 is the one you start the match with; the two reels never show the same weapon.
- **Ready up:** tap **READY UP** and the reels turn into **WAITING FOR GAME START**. On the host phone, **START** sits next to it and starts the match right away. **← Change tank** takes you back to the reels.
- **Control settings:** the gear at the top right (**CONTROLS**) opens your control settings at any time, before or after you ready up. They're saved on that phone:
  - **Quick weapon swap:** double-tap the driving side of the screen to swap weapons, instead of using the weapon button above BOMB.
  - **Sides:** drive on the left and aim on the right (the normal way), or swap them: aim on the left, drive on the right. The BOMB and weapon buttons move to the aiming side.

### Phone controls

- **Left half:** put your thumb down anywhere and slide. Left and right drive. **Push up to fire the jetpack.** Pull down to drop through a floating ledge.
- **Right half:** drag in the direction you want to shoot. The farther you drag, the more power. **Let go to fire.** A quick tap fires your last shot again.
- **BOMB button** (bottom right, unlimited bombs): put your thumb on it and drag, just like aiming a missile. The farther you drag, the harder you throw, and the host’s screen shows where the bomb will land. **Let go to throw.** A quick tap without dragging drops a mine under your tank.
- **Weapon button** (above BOMB): tap to swap between your two weapons (see *Weapons*). It shows the one you have. With **quick weapon swap** on, double-tap the driving side instead.
- The left and right halves swap over if you picked **aim left · drive right** in the control settings.
- **AIR STRIKE button** (next to BOMB): appears when you grab an air strike. Tap it, then steer the big red target on the TV with the left stick and tap **LAUNCH**.
- **Sound** (in the lobby menu, the **⋯** button): your phone plays its own sounds when your tank gets hit, knocks someone out, grabs a power-up or goes down. iPhones stay silent when the ring/silent switch is set to silent.

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

Bombs fly the way your barrel points, so aim with the barrel keys while you hold the bomb key. A quick tap of the bomb key drops a mine. With the machine gun, hold the fire key to keep firing. **P** pauses (or click the **PAUSE** button at the top left of the screen during a match), and so does Esc; M mutes. The pause key works for everyone at the keyboard and can be changed like any other key.

### Change any key

Every keyboard key can be changed. Open settings (the gear at the top right of the lobby, or **KEYS** on the pause screen) and click **Customize keys**. Click the key you want to change, then press the new one. If another action already uses that key, the two swap, so nothing ends up on two jobs. Esc cancels, and **Reset to default** puts everything back. Your keys are saved on this computer, and the lobby hints and the controls list (the keyboard icon) always show the keys you picked. Esc (pause), M (mute) and Enter (start) can't be used.

### Mouse or trackpad aiming

One keyboard player can aim with the mouse or trackpad. It's Keys 1 to start with; change it (Keys 1, Keys 2 or Off) under **Mouse aims** in settings or in the Customize keys window.

- **Point** to aim: the barrel follows the pointer. The farther the pointer is from your tank, the more power.
- **Click** to fire. Hold the click to see where the shot will go, then let go to fire. With the machine gun, hold the click to keep firing.
- **Right-click** (a two-finger click on most trackpads) drops a mine. Hold the right button to throw a bomb toward the pointer instead. The bomb key still throws along the barrel too.
- **Air strike:** the big target follows the pointer; click to launch.

The keyboard keys keep working alongside the mouse, and the pointer is a bigger red target, so it's easy to see.

### Game controllers

Game controllers join with A. Left stick drives (A or LB for jetpack), right stick aims and sets power, RT or RB fires (hold it with the machine gun). B throws bombs: hold the right stick in the direction you want and hold B, then let go of B to throw, or tap B with the stick centred for a mine. Y swaps between your two weapons (in the lobby it changes which two). X calls an air strike: move the target with the left stick, then press X or RT to launch.

### Rules

- Everyone has the same number of lives, **3** unless you change it (or unlimited respawns in a timed match).
- Missiles and bombs drain health. A **direct hit** does the most damage; near misses do less the farther away they land.
- Every hit **knocks you back**, and the less health you have, the farther you fly. Each player's card shows a **knockback multiplier**: ×1.0 at full health, about ×2.2 at half and nearly ×4 when you're almost out. It turns red at ×2 or more.
- Your **jetpack** has about 3.5 seconds of fuel and **refills the moment you land**. Use it to reach higher levels and to fly back after a big knockback.
- Falling off the map is **instant death**: you lose a life no matter how much health you had.
- Running out of health also costs a life. You respawn at the top after a couple of seconds, invincible for about 3 seconds.
- **Combos:** hit the same tank again before it lands and settles and the hit does more damage: ×1.25 for the second hit, ×1.5 for the third, up to ×2. The hit shows **2 HIT COMBO**, **3 HIT COMBO** and so on. Only hits from the same player (or CPU) count, so hits from different players never add up to one combo. For example, bomb a tank into the air, then snipe it before it lands, and the snipe does extra damage.
- **KO streaks:** knock out another tank within 7 seconds of your last knockout and the game calls it out over your tank: **DOUBLE KO!**, **TRIPLE KO!** and so on.
- While you wait to respawn, your card counts down the seconds until you're **BACK IN**. Once you've lost your last life it says **OUT**.
- A tank that gets knocked flying leaves a short trail in its colour, and every tank has a soft glow on the ground under it in its player colour, so you can always find yours, even in the air.
- Who goes down and who grabs a power-up shows near the top of the host’s screen, small enough to stay out of the way.
- The camera only zooms in and slows down for the **final knockout** of a match. The screen shakes when tanks get hit, and shakes less the more tanks there are, so an 8-player brawl stays easy to watch.

### After the match

The results screen shows who won, a scoreboard for every player (lives left, knockouts, falls, damage, direct hits, bomb hits and missile hit rate) and up to four awards: **Most damage**, **Most KOs**, **Sharpshooter** (best hit rate, with at least 5 shots), **Bomb expert** and, with power-ups on, **Collector**. **Rematch** plays the same setup again; **Back to lobby** lets everyone change tanks and settings.

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
| ◆ Missile | Arcs; drag farther (or charge longer) for more power | 21 direct, splash around the blast | About 1.1 seconds |
| ≡ Machine gun | A stream of fast rounds while you hold the aim; just point it | 4 per round, no splash; each round pushes a little | About 9 rounds a second |
| ⊕ Sniper | A very fast, almost straight shot | 48 direct, small blast | About 2.1 seconds |
| ⬤ Bazooka | A slow, heavy rocket with a high arc | 34 direct and a huge blast radius with big knockback | About 2.8 seconds |

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

There are seven arena types, and each one comes in three sizes: **Small**, **Big** (about double) and **Mega** (huge, for up to 8 players). Every type changes the game in its own way, and each has its own look: grass and layered rock, packed snow and ice, steel tread plate, space-station panels, sand and sandstone, or city rooftops. Busy backgrounds (the city windows in Neon City and Magma Foundry, for example) are toned down so the platforms you drive on stand out.

The game adjusts its resolution as it runs to stay smooth, so it plays well on older computers and on phones as well as on a big TV.

| Type | Small | Big | Mega | What's special |
|---|---|---|---|---|
| Skyforge (grass) | Skyforge Isles | Skyforge Archipelago | Skyforge Expanse | **Earthquakes:** every so often the ground rumbles, then the islands shake for a few seconds and bounce the tanks around. Careful near the edges. |
| Frostpeak (ice) | Frostpeak Basin | Glacier Fortress | Frostfall Citadel | **Sheet ice:** let go of the stick and a tank slides a long way (it sprays ice as it goes), and it takes a while to turn round. Weight counts: at the same speed a heavier tank slides further and is slower to turn round. |
| Magma (fire) | Magma Foundry | Magma Refinery | Magma Inferno | **Volcano bounce pads** (glowing pads with arrows rising out of them) throw any tank that drives or lands on them sky-high, with a full jetpack. A pad throws you about **two levels up**, on every map type, leaving a trail of fire. Every few seconds a pad also rumbles and erupts in a column of fire that burns and launches whoever is on top even higher. |
| Titan (space) | Titan Outpost | Titan Orbital | Titan Megastation | **Low gravity** (about 40% of normal): tanks float up and drift down, knockbacks carry much further, and shells fly in long, floaty arcs. Light tanks float longest; heavy ones come down sooner. |
| Warp (portals) | Warp Junction | Warp Nexus | Warp Labyrinth | Linked portals (shown by colour) teleport tanks, missiles and bombs. A portal goes dark when the platform under it (or under its partner) is gone. The camera holds still so teleports don't make it jump. |
| Abyss (underwater) | Coral Reef | Sunken Ruins | Abyssal Trench | **Deep water:** tanks are buoyant and sink slowly (trailing bubbles), missiles arc gently but slow down fast, bombs drift and sink, and a strong current drifts back and forth, pushing tanks and shots with it. Light tanks float longer and get pushed around more by the current; heavy tanks sink faster and hold their ground. |
| Neon City (city) | Neon Rooftops | Neon Boulevard | Neon Megacity | **Fog** rolls in every so often, thick enough to hide the whole background and the platforms for a few seconds. They're still there, so remember where they were. Tanks, bombs and power-ups stay visible. |

**Map type** (pick one; only one can be on at a time):

- **Regular:** the arena as it is, with its own twist (see the table above).
- **Classic:** no twists at all: no bounce pads, fog, earthquakes, portals, slippery ice, low gravity or water. Just the platforms.
- **Bounce:** a glowing energy net stretches under the arena. Fall into it and it throws you back up with a full jetpack, but every bounce costs 30 health (and can knock you out if you're low). Fly off the sides past the net and you still fall. Bombs and missiles explode on the net.
- **Active:** the map changes while you play. Every 11 to 17 seconds something happens. There's no warning banner: each event has its own signature sound (a howling wind, a rumbling avalanche, bubbling lava, horns of hover traffic and so on) that starts a second or two before it hits, so you can hear it coming. Half the time a group of platforms (the left side, the right side, the top platforms or the bottom decks) blinks red, crumbles away, and comes back about 6 seconds later, so get off them when they blink. The other half is the arena's own event:

| Type | Active-map event |
|---|---|
| Skyforge | **Wind gust:** a strong wind blows everything one way for a few seconds. |
| Frostpeak | **Avalanche incoming:** a wall of snow sweeps across the high or low half of the map, hitting and shoving every tank in its way. |
| Magma | **Lava is rising:** the lava climbs up over the bottom decks, holds there, then drains. Touching it burns and throws you upward. |
| Titan | **Meteor shower:** meteors rain down and explode where they land. |
| Warp | **Portals haywire:** every portal leads somewhere random for a few seconds. |
| Abyss | **Tidal surge:** a powerful current pushes everything one way. |
| Neon City | **Hover traffic:** a stream of flying cars sweeps across the high or low half of the map, hitting and shoving every tank in its way. |

- **Rising:** the whole map keeps climbing. A few seconds into the match a deep rumble plays and a hazard that matches the arena starts rising from the bottom, and the view (and the edge you fall off) climbs with it. There are only ever **four levels** of platforms: each time the hazard swallows the bottom one, a new level drops in at the top with a flash, so you can see where to go next. Platforms flash before they're swallowed. **Touching the hazard knocks you out**, just like falling off the map (if someone hit you just before, they get the knockout). The camera always keeps the hazard in view, and it rises a little faster the longer the match goes on. You respawn on one of the top platforms. Big and Mega maps start with only their lowest few levels.

  The arena's own twist keeps going as the map climbs: on Magma nearly every new level has a volcano bounce pad (two on wide maps once the match is a minute in), and on Warp new levels bring new pairs of portals, more often as the match goes on.

| Type | What rises |
|---|---|
| Skyforge | **Earthquake:** the islands shake apart from the bottom up. The lowest ones shake hard, then crumble away. There's nothing underneath, so dropping below them knocks you out. |
| Frostpeak | **Snow:** a snowdrift buries the lowest ledges. |
| Magma | **Lava:** lava swallows the lowest decks. |
| Titan | **Meteor belt:** a band of tumbling rocks climbs through the station. |
| Warp | **Warp storm:** a crackling storm swallows the lowest levels and switches off the portals on them. |
| Abyss | **Riptide:** the tide floods the lowest shelves. |
| Neon City | **Toxic fog:** the fog swallows the lowest rooftops, and you can't see platforms inside it. |

CPU players know what's coming too: they get off dropping platforms, away from rising lava, and on a rising map they keep climbing.

Mega maps are wide, so with everyone spread out the camera pulls back a long way and tanks look small. They play best on a big TV.

### Tanks

In the lobby, each player's tank turns slowly on a turntable. Each tank has its own look, but every tank is the same size and uses the same missiles, bombs and jetpack. They differ in these stats (the phone's **?** card shows them):

| Tank | Role | Strengths | Trade-offs |
|---|---|---|---|
| Vanguard | All-rounder | Even in every stat | No standout strengths |
| Striker | Scout | 25% faster, 25% more jet fuel, slightly quicker reload | 10% less health, easier to knock back |
| Bulwark | Heavy | 28% more health, 28% harder to knock back, 5% more damage | 20% slower, reloads 15% slower, 15% less jet fuel |
| Ravager | Demolition | 15% bigger blasts, 10% more damage, 12% more knockback | Reloads 10% slower, a little slower to drive |
| Viper | Rapid fire | Reloads 26% faster, faster missiles | 20% less damage, 10% less health, smaller blasts |

**Weight** matters in the arenas with a twist. From lightest to heaviest: Striker, Viper, Vanguard, Ravager, Bulwark. On ice a heavier tank slides further (for its speed) and is slower to turn round; in low gravity a lighter tank floats longer; underwater a lighter tank sinks more slowly and gets pushed around more by the current. A tank shrunk by the **Tiny** power-up counts as much lighter for all of these.

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

