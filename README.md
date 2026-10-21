# Rotorwash

A browser helicopter trainer for practising Battlefield-style flying and aiming on a PC without a discrete GPU. One self-contained page (`index.html`) built on three.js r128, loaded from cdnjs.

## Run

Open `index.html` through any local web server, for example:

```
python -m http.server 8765
```

then browse to http://127.0.0.1:8765/. Click **Fly**, then click the view to capture the mouse. Esc pauses.

## Default controls

All of these can be rebound in the menu's **Controls** tab. Pitch, roll and yaw each take a key pair or a mouse axis. Bindings are saved in the browser.

| Input | Action |
|---|---|
| W / S | Throttle up / down |
| Mouse X | Yaw |
| Mouse Y | Pitch |
| A / D | Roll |
| Left / right click | Gun / rockets |
| C | Chase or cockpit camera |
| Hold R | Respawn on the home pad |
| H | Show / hide help |

## Drills

- **Free flight:** 12 target vehicles to shoot, marked in red.
- **Ring course:** 10 rings against the clock, best time kept.
- **Landing drill:** pads A, B, rooftop C and home in turn, each landing graded by touch-down speed.

## Tuning

Every flight, weapon and camera constant is in the `TUNING` object at the top of the script.
