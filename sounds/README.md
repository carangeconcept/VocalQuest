# Custom sounds for Vocal Quest

The game makes its own sounds. To replace any of them, put audio files
(mp3, wav or ogg) in this folder and list them in `pack.json`:

```json
{ "win": "victory.mp3", "alarm": "parry-shout.mp3", "lvl": "level-up.mp3" }
```

Anything you leave out keeps its built-in sound. Keep clips short.

| Name | Plays when |
|---|---|
| `tap` | a menu button is pressed |
| `count` | each tick of the 3-2-1 before a spell |
| `go` | the countdown ends |
| `cast` | a note is sung well enough to cast (muted while you sing) |
| `miss` | a note or answer is missed |
| `alarm` | a foe throws a note back (parry) / Blind Note asks its question |
| `right` | a tap answer is correct |
| `perfect` | a foe is destroyed, or a dead-on echo |
| `win` | victory screen |
| `lose` | defeat screen |
| `star` | each star stamped on the victory screen |
| `lvl` | level up |
| `coin` | gold or a daily job is paid |
| `chest` | a crate is opened |
| `equip` | gear equipped, stat point spent, tea drunk |
| `gate` | a Sky Glide gate is passed (muted while you sing) |
| `crash` | a Sky Glide gate is hit (muted while you sing) |
| `menu` | the theme loop on menus; it fades out whenever a note plays or the game is listening |

## Guide sounds

The note you copy in lessons and games is the **guide**, chosen under Hero → Guide sound:

- **Voice** (default): a built-in sung "ah" tone, easiest to match.
- **Flute**: a pure built-in tone.
- **Piano** and **Cello**: Suno samples listed in `inst/samples.json`. Each entry gives the
  file and its measured pitch as a MIDI number (60 = middle C). The game plays the nearest
  sample and retunes it to the exact pitch. The cello samples stop at G3, so its high notes
  sound an octave lower (still the same note name).

All files in this folder were generated with Suno.
