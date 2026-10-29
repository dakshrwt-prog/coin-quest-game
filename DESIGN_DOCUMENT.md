# Coin Quest — One-Page Game Design Document

**Genre:** 2D arcade collection / survival  
**Audience:** Beginners and casual players, approximately ages 8+, who enjoy short reflex games.  
**Platform:** Desktop and mobile web browser  
**Session length:** 45 seconds per round

## Goal
Collect **10 gold coins** before time runs out while avoiding moving red hazards.

## Core loop
1. Start a round.
2. Move the mint-green player around the arena.
3. Touch gold coins to gain one point; a sparkle burst confirms collection.
4. Avoid red hazards. A collision removes one of three lives and briefly grants invulnerability, shown by blinking.
5. Win at 10 coins. Lose if time reaches zero or all lives are gone.
6. Read the result message and play again.

## Rules and feedback
- The target is 10 coins; the timer begins at 45 seconds.
- Three lives are available.
- Coins respawn after collection; hazards bounce around the arena.
- Coin collection updates the score and emits gold particles.
- Hazard contact updates the hearts and makes the player blink.
- Win and lose states use clear text and a replay button.

## Controls
- **Keyboard:** Arrow keys or WASD to move.
- **Mobile:** On-screen left, up, and right buttons. (The up button moves the player upward.)
- **Restart:** Click “Play again”; press R after a round ends.

## Scope and placeholder art
All visuals are simple circles, grid lines, and emoji/text UI. This intentionally keeps the prototype small and testable.

## Success criteria / playtest
- A new player can start within 10 seconds without instructions from the designer.
- Coin pickups increase the score exactly once each.
- Hazard collisions reduce lives without draining all lives in a single overlap.
- Reaching 10 coins shows the win state; reaching 0 seconds or 0 lives shows the lose state.
- Restart resets score, timer, lives, coins, and hazards.
