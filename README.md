# MultiChess (Windows)

A desktop chess game built with Python and Tkinter. Play against the built-in chess bot or play another person online.

## Features

- Human vs. computer, with an adjustable bot strength from Elo 400 to 3200.
- Online multiplayer through the project's WebSocket server.
- Chess rules including castling, en passant and promotion.
- Sound effects for moves, captures, castling, checks and game end.

## Run from source

Requires Python 3.12 and Tkinter.

```powershell
py -3.12 -m pip install websockets
py -3.12 MultiChess.py
```

Tkinter is included with most standard Windows Python installations. If it is missing, install the Python Tcl/Tk component.

## Build the Windows executable

The **Build Windows Executable** GitHub Actions workflow builds a standalone `MultiChess.exe` with PyInstaller. Run it from the Actions tab or push a change to `MultiChess.py`, `chess/`, or the workflow file. Download the `MultiChess-Windows` artifact from the completed run.

Online multiplayer requires the hosted WebSocket server to be available. The local bot does not depend on that server.
