# Glass Poker <img width="768" height="1376" alt="579AA696-707F-405B-A3E4-491235F85F69" src="https://github.com/user-attachments/assets/55cc36d7-7fd4-4641-8df4-6c82676d44c8" />
<img width="768" height="1376" alt="579AA696-707F-405B-A3E4-491235F85F69" src="https://github.com/user-attachments/assets/a20b26d2-c956-42b4-a8e1-577a34f44221" />


Glass Poker is a minimalist, single-handed web application for playing poker (Texas Hold'em) against AI opponents. The entire interface is built upon a modern, high-resolution liquid glass design (glassmorphism), creating a clean depth effect through semi-transparent surfaces, background blur, and soft borders.

## Features

### Liquid Glass Interface
The entire user interface completely dispenses with classic neon effects or distracting banners. All menus, buttons, overlays, and the navigation are implemented as functional glass elements using backdrop filters. The navigation icons are uniformly designed in pure white.

### Automated Gameplay
The player always acts first in every betting round (Pre-Flop, Flop, Turn, River). Following the player's action, all active AI bots execute their moves fully automatically one after another with a brief built-in delay. Once the round is completed, the next phase loads seamlessly without requiring manual intermediate steps.

### Swipe-to-Fold Gesture Control
Traditional fold buttons have been entirely removed. Discarding weak hands is done via a direct swipe gesture. Cards are dragged upward by touch or pointer, visually flying onto the table to trigger the fold action. This is achieved using the PointerEvents API with pointer capture to prevent accidental browser scrolling.

### Tactical HUD Display
Located directly next to the primary action buttons (Call and Raise) is a permanent informational box. This box calculates and displays your statistical win probability in real time for the current phase of the game.

### Visual Rules Overlay
Clicking on the community cards opens a full-screen glass panel. This overlay contains a comprehensive guide to all poker hand rankings, visualized with miniature rendered playing cards as direct image examples.

### Full Table Setup & Bankroll Vault
Before entering a game, a glass slider allows you to easily adjust the stakes (blinds) and view the corresponding buy-in. Through the vault area, a simulated top-up system is available, displaying the acquisition of new test chips with a full-screen loading and confirmation animation.

## Technical Details

* Architecture: Single-Page Application (SPA)
* Technologies: HTML5, CSS3 (Flexbox, CSS Grid, 3D Transforms), JavaScript (Vanilla ES6)
* Input Handling: PointerEvents API for precise gesture recognition on mobile devices and desktop browsers
* Design System: Pure glassmorphism via advanced CSS properties (backdrop-filter)

## Installation and Setup

Since the project consists entirely of client-side code, no installation or local server environment is required.

1. Clone the repository:
   git clone https://github.com/poicpp/glasspoker.git

2. Navigate into the directory:
   cd glass-poker

3. Open the index.html file directly in any modern web browser of your choice.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Play

Hit that Link to play Glass Poker V.1.0: https://poicpp.github.io/Glasspoker/
