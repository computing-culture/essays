## Worked Example: Unreal (1998)

To show how the structure works in practice, this section walks through the original Unreal using the reconstruction method.

### 1. Software Anchor

Before widespread broadband access, many PC games emphasised single-player exploration and atmosphere. Dark hostile worlds were a popular genre. Unreal left a much bigger social memory than other games that shared this aesthetic, such as earlier "Into the Darkness (Mac)" and later "Aliens vs Predator (PC)".

Unreal was released in 1998 as a first-person shooter focused on exploration, atmosphere, and precise but not twitch-heavy combat. Its pace is slower and more deliberate than many shooters, with long sight-lines, vertical spaces, world immersion, immersive audio cues, and the dark hues from which polygon threats emerge.

Characters could shoot an alien disc weapon (Razorjack) that launches spinning discs with full 3D trajectories, 3D wall ricochet, and timed directional sounds. This means 3D audio and 3D visuals are tightly coupled. And, it means players have time to position themselves horizontally or vertically where they think the spinning blade is least likely to pass.

The goal is not to ask what hardware can run Unreal today, but what kind of human–machine system Unreal expected at the time it was designed.

### 2. Expected Interaction (HCI)

Unreal assumes a player who:
Uses continuous mouse movement to discover a world with rotations, rather than very fast snap movements. Relies on spatial awareness when reacting to emerging threats. Combat rewards 3D movement as much as instant reaction.

### 3. Input and Display Assumptions

**Mouse:** Mechanical ball mouse

* Small corrections are harder than 360 rotations.
* Lifting and re-centering are normal.

**Display:** 4:3 CRT

* Centralized field of view
* Reinforces strong 360 motion persistence

These conditions encourage sustained tracking rather than fast snap aiming.

### 4. Graphics and Audio APIs

**Graphics:** Glide/DX5

**Audio:** CD-quality audio. DirectSound3D (optional A3D) - positional cues are important.

Timing is stable and predictable, which supports spatial sound and movement cues that encourage users to listen for audio details - not treat it as atmospheric background music.

These APIs encode assumptions about timing, lighting complexity, and spatial sound that shape how the game feels moment to moment.

### 5. Anachronisms to Consider

Several modern substitutions quietly change the experience:

15" CRT was mainstream, and 14" LCD panels existed as an alternative. But, behaviours of LCD panels were vendor-specific, some emulated CRT better than others, and none matched the dark hues common to CRTs that Unreal exploited.

Adopting an unforgiving 14" LCD panel demanded more of the graphics card - higher resolution and greater bit depth. That's plausible for a top-end workstation in 1998.

High-DPI optical mice changed the input motion, and broke full-circle 360 scanning with spinning ball inertia. An original ball mouse would operate on serial/PS2, while an optical operated on USB.

Microsoft Windows audio engines increasingly rely on software mixing and resampling, which can subtly change timing and reduce the tight coupling between sound and motion that Unreal relies on.
Furthermore, Unreal's audio was optimised for A3D, which had full official support on Win95/Win98/WinME and Windows NT 4.0 only.

Unreal targets 3Dfx Glide, which is consistently efficient across all operating systems and itself targets CRT displays.

For comparison, Microsoft's later Direct3D APIs are backwards compatible, but there is an overhead to orchestration such that running a DX5 game on DX9 runtime shouldn't change the images but will increases the stress on CPU caches and doing that can increase frame drops.

These changes may alter difficulty, pacing, spatial awareness, and immersion - by changing how the player moves, listens, and predicts space.

So what was realistic in 1998?

The actual most efficient code path would be 3Dfx Glide. And, any 3Dfx card of the era lacks bandwidth to properly drive 1024x768x32 on a 14" LCD, which explains why Unreal more often paired 800x600x16 on 15" CRT.

The next most efficient code path would be DX5 drivers on DX5 runtime, which is only possibly on Win95/Win98 or Windows NT 4.0. Driver requirements match the Nvidia TNT (TNT2 requires DX6 runtime).

### 6. Did Such A Machine Exist?

Unreal was rarely bundled with complete OEM PCs, but was commonly used as a showcase title in 3Dfx graphics card bundles. This positioned Unreal as the demonstrator of 3Dfx's interactive media capabilities.

Plausible lower end 1998 gamer configuration: 3Dfx Voodoo 4Mb (analog out), Microsoft Intellimouse, 15" CRT (640x480x16 analog in), Ensoniq AudioPCI. This configuration was buildable, usable, and matched Unreal’s target audience.

Plausible upper end 1998 gamer configuration: 3Dfx Banshee 16Mb (analog out), Microsoft Intellimouse, 17" CRT (800x600x16 analog in), Aureal Vortex. This configuration was buildable, usable, and matched Unreal’s target audience.

Plausible alternative Direct3D configuration: TNT 16Mb (analog out), Microsoft Intellimouse, 12" LCD (800x600x32 analog in), Aureal Vortex. This configuration was less common but doable.

And, these system-level constraints expose a truth of 1998 and Unreal's launch environment: The most powerful Direct3D cards lacked bandwidth to properly drive 1024x768x32 on a 14" LCD, which cements why Unreal more often appeared at 800x600x16 on 15" CRT.

### 7. Did It Last Long Enough to Matter?

The HCI that Unreal was optimised for existed for almost a decade (1990-2000).

Unreal launched in 1998 and was displaced in first-person multiplayer shooters by Unreal Tournament in 1999. But as single-player game Unreal remained culturally present through the transition to LCD displays, hardware T&L GPUs, and optical mice. The shared Unreal Engine was reused and expanded in many later games.

This longevity meant that the interaction style Unreal assumed had time to be learned, practiced, and remembered irrespective of CPU, RAM and disk drives - these components have not emerged as primary constraints because they are not directly shaping player behaviour or interaction style.
