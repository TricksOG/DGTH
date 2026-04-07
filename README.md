What is this?
DGTH is a browser game built around a real theory about how consciousness works — the Density-Gated Traversal Hypothesis. The game is a single HTML file, zero dependencies, zero build step. Open it and play.
It started as a snake game. It became something stranger.
The core idea: what if your mind isn't generating thoughts, but traversing a substrate of information that already exists in full? Every idea, every memory, every feeling — already there. You are the worm. The dark grid is everything that could ever be known. You move through it. You don't write it.
That's not just flavor text. Every mechanic in the game maps directly to a piece of the theory.

The Theory → The Game
Theory primitiveWhat it isIn the gameΩ (Omega)The substrate — complete, unchanging, infiniteThe dark grid. It was always there.CConsciousness — the traversing awarenessYour worm. You move through, not create.FThe filter — direction of attentionThe direction you're facing. You can only absorb what's ahead.ITIntersection Topology — zone boundariesSeam Events. Cross a zone border, something clicks. +50.
Dense (dark) cells — high information density. Slow to traverse, worth more points. Hard thoughts take time.
Visited cells — softened, lighter. You were here. The path stays open. Moving faster through known territory.
Locked red zones — knowledge gated by traversal depth. Score more, unlock more.
Filter Capture — the failure mode. You stop exploring. You loop. Three captures and it's over.

Gameplay
DGTH plays like a territory-coverage game, not a pure snake. You and an AI opponent both traverse the same substrate. The goal is to cover as much ground as possible before time runs out — or eliminate your opponent with three Filter Captures.
Modes

Solo — you against the clock, no opponent
VS AI — competitive traversal against an AI worm
Campaign — five levels with escalating mechanics, starred completion, unlockable raids
Raids — three boss encounters (VORRAX, XORRATH, MALGATH) that actively devour the substrate as you fight to cover it

Difficulty
AI speedCapture timerNoiseVoid pulsesNormal0.82×11sHighNoneHeroic1.15×7sLowNoneMythic1.15×7sLowYesLegendary1.15×7sLowFrequent
Controls
Desktop — Arrow keys or WASD
Mobile (portrait) — Virtual thumbstick below the canvas, or swipe anywhere on the canvas

Campaign Levels
#NameMechanic1GenesisStandard substrate. Learn the fundamentals.2The LabyrinthDense locked zone coverage. Narrow corridors.3The DeepMaximum density throughout. Enormous score multipliers.4The FractureBoard fractures at 90 seconds. Zone topology scrambles.5The CrucibleIsolation boxes dissolve at 60 seconds. Then war.

Raids
Three boss encounters unlocked after earning 8 campaign stars. Each boss actively devours the substrate — the board gets smaller as you fight. Cover enough of what remains to win.
VORRAX — The Devouring Flame
3×3 boss. Void Breath sweeps 3-cell-wide corridors. Fragment Spawn drops void cells across the board.
XORRATH — The Omnivoid
4×4 boss. Void Gaze rotates a beam across the board. Tendrils creep inward from all edges. At 35% devoured, controls invert for 3.5 seconds.
MALGATH — The Entropy Deceiver
6×4 boss. Three escalating phases. Void Shatter, Entropy Bolts, Nullspace darkness. Enrages at 3 minutes.

Power-ups
Effect🟢 BOOSTSpeed surge for 4 seconds🔴 BOMBStuns opponent for 2.5 seconds🟡 SHIELDAbsorbs the next Filter Capture🔵 FREEZESlows opponent for 3 seconds🟣 SCRBLScrambles opponent's filter direction🩷 +HPRestores 35 HP (raid mode only)

Technical

Single HTML file — no framework, no bundler, no CDN calls during gameplay
Canvas rendering — physical pixel buffer matches display resolution × device pixel ratio, eliminating CSS upscale blur
Web Audio API — fully procedural music engine. Every track is composed as note sequences and scheduled in real time. No audio files.
Mobile — virtual thumbstick with deadzone, cardinal snap, and glowing arc direction feedback. Score strip HUD below canvas. Portrait-native layout.
Particle system — burst effects on traversal, seam events, power-up collection, screen shake and damage vignette on hits

Music tracks
Each game state has its own composed track: title, level select, raid select, five campaign levels, three raid encounters. All generated from note arrays at runtime using oscillators, gain envelopes, and scheduling loops.

Origin
Written in February 2026. One human, three AI systems (Claude, ChatGPT, Grok), iterating together across many sessions. The theory came first — a metaphor about consciousness as non-linear traversal of pre-existing information. The game came second, as a way to make the theory playable.
The framework has been formally documented. This is the playable version.
