# Welsham Railway

A browser-based train driver simulator running the **Welsham Circle** — an
8-station circular urban route — driving the **Class 700/0** Thameslink
Desiro City. Forked from the
[Yorkshire Train Simulator](https://github.com/BrendanJamesLynskey/Airedale-Wharfedale-Sim)
with the bundled maps and rolling stock pruned down to just this single
line and unit.

[Play it here](https://brendanjameslynskey.github.io/Welsham-Railway/)

## Route

**Welsham Circle** — 22.9 km, 8 stations, urban biome.

| # | Station | Code | km | Sched |
|---|---------|------|----|-------|
| 1 | Welsham Central | WEC | 0.00 | 00:00 |
| 2 | Welsham Jn | WEJ | 2.97 | 03:28 |
| 3 | Silkie Street | SIK | 7.84 | 08:50 |
| 4 | Bankside | BNK | 10.10 | 11:36 |
| 5 | Welsham UFC | WFC | 13.28 | 15:16 |
| 6 | Welsham St Peters | WSP | 19.15 | 21:38 |
| 7 | Central Market | WCM | 20.78 | 23:46 |
| 8 | Welsham Central | S08 | 22.92 | 26:24 |

Speed limits: mostly 60–75 mph with 50 mph through the central section
around Welsham UFC. Features include a 400 m tunnel near km 5, three
bridges (km 10.1 / 10.5 / 20.1), an 80 m viaduct at km 16.8, and a mill
on the right at km 19.2. The river crosses the line near Bankside.

The track geometry is loaded from [`welsham-circle.json`](welsham-circle.json),
which is the same route file format used by the parent sim's `LOAD FROM FILE…`
loader and the
[Yorkshire Line Editor](https://github.com/BrendanJamesLynskey/Yorkshire-Line-Editor).

## Rolling Stock — Class 700/0

The only drivable unit. 8-car Siemens Desiro City, 162.6 m, 388 t,
**central** driving position (unusual for UK stock), MITRAC IGBT inverter
audio (350 Hz → 1400 Hz sweep), 1.0 m/s² acceleration, 1.2 m/s² service
brake. Bespoke cab interior: large central DMI, slim TMS and ETCS screens
flanking it, CCTV monitor strip above the windscreen, master controller to
the driver's right, AWS / DRA / EBP cluster further right, TPWS panel on
the left.

## Controls

| Key | Action |
|-----|--------|
| `↑` / `↓` | Notch power up / brake on |
| `Space` | AWS reset (acknowledge audible warning) |
| `D` | DRA toggle |
| `H` | Horn |
| `Tab` | Cycle HUD overlay |
| `C` | Toggle free-cam (WASD / Space / LCtrl to fly, drag to look, C again to return) |
| `Esc` | Quit to menu |

## Repo

[BrendanJamesLynskey/Welsham-Railway](https://github.com/BrendanJamesLynskey/Welsham-Railway)

## Licence

MIT.
