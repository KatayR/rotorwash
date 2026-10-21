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
| Hold R (tap after a crash) | Respawn on the home pad |
| H | Show / hide help |

## Flight models

Pick one on the menu's **Fly** tab.

- **Battlefield:** throttle is momentary. Hold it to climb or sink, and let go to settle into a slow sink.
- **More realistic:** throttle moves a collective lever gradually, and the lever eases back to the middle (a slow sink) when both keys are released. Rotor thrust lags the lever, power changes yaw the nose through main-rotor torque, there is translational lift at speed, and the helicopter carries more momentum. Its constants are in the `REALISTIC` object.

## World

A 3 km square map with mountains at the edges, a round town about 635 m across with towers up to 110 m, three ground pads and a rooftop pad.

## Drills

- **Free flight:** 12 target vehicles to shoot, marked in red.
- **Ring course:** 13 rings in one smooth loop against the clock, best time kept.
- **Landing drill:** pads A, B, rooftop C and home in turn, each landing graded by touch-down speed.

## Tuning

Every flight, weapon and camera constant is in the `TUNING` object at the top of the script, and the realistic model's overrides are in `REALISTIC` beside it.
