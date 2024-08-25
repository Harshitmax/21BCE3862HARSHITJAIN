Code Organization:
The project must be in a single repository with clear separation between client and server code.
Include a README with setup and run instructions for both client and server.
Server-side Implementation:
Implement the core game logic as described in the Game Rules section.
Set up a websocket server to handle client connections and game events.
Process move commands and update the game state accordingly.
Implement thorough server-side move validation.
Client-side Implementation:
Create a basic web interface that displays the 5x5 game board.
Implement websocket communication with the server.
Implement client-side move validation (mirroring server-side validation).
Display valid moves for the selected character.
Send move commands to the server and handle responses.
Websocket Communication:
Implement event handling for game initialization, player moves, and game state updates.
Ensure real-time synchronization of game state between server and all connected clients.
Move Validation (both client and server-side):
Prevent selection or movement of opponent's pieces.
Ensure moves are within the 5x5 grid boundaries.
Validate moves according to each character type's movement rules.
Prevent friendly fire (moving onto or through spaces occupied by friendly characters).
Handle and communicate invalid move attempts to the user.
Edge Cases to Handle:
Simultaneous move attempts by multiple clients.
Disconnection and reconnection of clients during an ongoing game.
Attempts to make moves out of turn.
Handling of game state when a player quits mid-game.
Proper game termination when all opponent's pieces are eliminated.
Game Flow:
Implement turn-based gameplay with clear indication of current player's turn.
Correct handling of piece elimination upon valid capture moves.
Proper game end detection and winner announcement.
Code Quality:
Write clean, well-commented code following best practices for chosen technologies.
Implement error handling and logging for both client and server.
