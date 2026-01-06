# Why Games Fade, and How to Restore Them

## Formats, constraints, and fair play: an analogy between tabletop games and PC games

Many tabletop games and PC games rely on formats: shared constraints that define what counts as fair, meaningful, and comparable play.

In tabletop games, formats are usually explicit. They are written into rules, tournament structures, or allowed component sets. In PC games, formats are often implicit. They emerge from hardware limits, performance envelopes, and the difficulty of optimisation rather than from formal rules.

This essay proposes that when these implicit constraints disappear, a PC game does not merely become easier or faster. It becomes a different game.

## 1. What is a format in tabletop games?

In tabletop play, a format defines the boundaries of play:

* which components are allowed
* which rules apply
* what counts as a legal move or configuration

Formats make skill visible and comparable. They ensure that players are competing within the same limits, even when strategies differ.

Examples include:

* fixed rule sets in board games
* tournament deck restrictions in card games
* time controls in competitive chess

Crucially, formats are not about restricting creativity. They are about preserving meaning. Without shared limits, outcomes cannot be compared, and mastery loses its shape.

## 2. What formats do in practice

Formats serve several practical functions:

* They bound power so that escalation does not dominate play
* They preserve balance between different strategies
* They make improvement legible to other players
* They support long-term communities by stabilising expectations

Breaking a format is not the same as playing better. It is changing the conditions under which the game operates. Once that happens, results no longer carry the same meaning.

## 3. PC games also have formats, but they are implicit

PC games also assume constraints, even when they are not written down.

These constraints may include:

* expected APIs and operating systems
* expected frame-rate ranges
* expected input sampling rates
* expected difficulty of hardware optimisation

Unlike tabletop formats, these limits are rarely enforced by the software. Instead, they are assumed by the developers and shaped by the technology available at the time.

As a result, PC game formats emerge socially:

* through shared hardware availability
* through tuning difficulty
* through community norms about what is reasonable or fair

## 4. Tuning as part of the format, not cheating

In many periods of PC gaming, tuning was expected. Adjusting hardware, drivers, and settings was part of participating fully in a game.

As long as optimisation required effort, knowledge, and tradeoffs, it functioned as in-format play. Players who tuned their systems were not breaking the game; they were mastering it.

The format remained intact while:

* performance gains were possible but limited
* improvements required work
* advantages were earned rather than automatic

---

## 5. Formats, limits, and DirectX as a selector

On PC, formats are rarely named, but they can still be selected.

One practical way players have implicitly selected formats is through the installed DirectX version, which acts as a coarse performance limiter. The important factor is the distance between the DirectX version a game targets and the DirectX version present at runtime.

This produces three broad format types, analogous to tournament formats in tabletop games.

### Type 3 — Strict

Game DX matches installed DX exactly.

This is a highly constrained format, similar to boxed, sealed, or archival play.

* Hardware is tightly limited
* Frame-rate ceilings are low
* Optimisation is minimal or impossible

This format preserves technical fidelity and original assumptions, but it is socially narrow and does not reflect how most competitive PC play actually occurred.

### Type 2 — Social

Game DX and installed DX are one generation apart.

This is the historically lived format for many PC games.

* Legacy paths still function
* Hardware is partially constrained
* Optimisation is possible but not trivial

Here, tuning is meaningful, effortful, and socially legible. Performance gains feel earned, and comparison between players remains fair. This is the window in which many PC games mattered most.

### Type 1 — Broken

Game DX and installed DX are separated by two or more generations.

In this format, power overwhelms structure.

* Driver stacks are rewritten for newer hardware
* Frame rates overshoot original envelopes
* Timing, physics, or input behaviour may drift

In tabletop terms, this is a broken or unlimited format: still playable and sometimes fascinating, but no longer comparable to earlier play. The game is not being played incorrectly, but it *is* being played under a different format.

---

## 6. Implications for preservation and history

This perspective has several important implications:

* Preservation: Preserving a game requires preserving its constraints, not just its software.
* Emulation: Accuracy without limits may reproduce code but not experience.
* Competitive fairness: Fair play depends on shared performance envelopes as much as on rules.
* Historical understanding: Many PC games mattered most within narrow windows where optimisation was meaningful but not trivial.

Freezing a hardware configuration captures a product. Preserving a format captures a practice.

## 7. Restoring games as constraint stacks

If formats explain why games fade, restoration requires a practical way to reintroduce those formats.

For PC games, this does not mean selecting a single "correct" machine. Instead, restoration can be understood as assembling a **constraint stack** that recreates the performance envelope in which the game’s interaction model once made sense.

A typical restoration stack proceeds outward from the game:

* **Game**: defines the interaction contract, control model, and physics assumptions
* **DirectX binary release**: constrains available APIs and acts as a coarse format limiter
* **Operating system version**: shapes scheduling, timing resolution, and background interference
* **Driver versions**: determine how much modern hardware capability is exposed or restrained
* **Chipset choices**: cap bus speeds, memory bandwidth, and I/O behavior

Taken together, these layers form a retro PC built *for the game*, rather than a historically generic machine.

Different choices within this stack legitimately produce different formats:

* strict or archival builds
* socially lived builds
* unlimited or broken builds

Console versions of games generally fall into the **strict or archival** category. Fixed hardware, capped frame rates, and locked driver stacks tightly constrain optimisation and preserve a narrow performance envelope. This can strongly support technical fidelity, but it also limits tuning and often prevents the kind of performance-driven competitive culture that emerged around PC games.

None of these are wrong, but they are not interchangeable. Restoration becomes meaningful only when the chosen stack—and therefore the chosen format—is made explicit.

## Closing thought

PC games fade not because they stop running, but because the constraints that once gave their play meaning quietly disappear.

Restoring them therefore requires more than compatibility. It requires rebuilding the constraint stacks that once bounded optimisation, made tuning matter, and allowed skill to be compared.

Formats, not specifications, are what make play fair and memorable.

## Citation

Computing Culture. *Why Games Fade, and How to Restore Them*.  
Computing Culture Essays, January 2026.  
https://github.com/computing-culture/essays
