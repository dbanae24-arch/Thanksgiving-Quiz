# Thanksgiving-Quiz

A live quiz. You host it on a big screen. Players scan a QR code and answer on their phones. No sign-in.

## Links (once it is on GitHub Pages)

- Players: https://dbanae24-arch.github.io/Thanksgiving-Quiz/
- Host: https://dbanae24-arch.github.io/Thanksgiving-Quiz/?host=ehy10o

The QR code on the host screen always points to the players link.

## Run a game

1. Open the host link on the big screen. The pill at the top right should say **Live**.
2. Players scan the QR code, type a name and tap Join.
3. Press **Start the quiz**. Space or the right arrow moves on.
4. To play again: **Menu > Start a new game**.

## What is in here

- `index.html` - the whole quiz (host screen and phone screen).
- `img/` - the five close-up pictures for round 2.

The questions are the `QS` list near the top of the script in `index.html`.

## How the phones reach the big screen

Messages go through three free public relay servers (MQTT over a secure WebSocket).
One server being down does not stop the game.

Nothing sent is private. Use first names only. Never put firm or client information in a quiz.

If the pill stays on "Connecting" on the office network, the network is blocking the relay servers.
Run the host screen from a phone hotspot or another network.
