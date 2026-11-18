[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/Harryyt01/news-image-20261118/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![reward](https://make.fun/badge/news-image-20261118/Harryyt01/news-image-20261118/reward.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)

# The World in One Day — make.fun "Sum up 18 November's world news in one image" entry

A newspaper front page for Wednesday 18 November 2026, drawn as one
1024×1024 image. Six stories, all reported that day:

1. **The Gulf crisis** — the US sinks five Iranian tankers; Iran hits
   back with drones on US radar sites in Bahrain and missiles at a base
   in Jordan.
2. **Ukraine hits the Kerch Bridge again** — a second night of strikes
   on the Crimea link as Russia pounds Kyiv's bridges.
3. **Gaza: UN warns of cold deaths** — floods swamp tent camps while
   four nations urge Israel to let aid through.
4. **COP31: final days** — climate talks in Antalya deadlocked over 144
   disputed items.
5. **Quad talks in Manila** — Trump lands for Quad talks ahead of a
   China visit; APEC meets in Shenzhen.
6. **North Korea fires a missile** — a ballistic missile flies into the
   Sea of Japan, Seoul says.

The four large illustrations are original flat editorial art made for
this entry; the two small panels (summit flags, missile) are drawn with
PIL shapes. All on-image text is rendered with PIL, so every word is
spelled correctly — no AI-generated text anywhere.

## How it works

`main.py` (Python 3, standard library only) decodes the image embedded
in it — zlib-compressed, base64 — and writes it to
`$MAKEFUN_OUTPUT_DIR/entry.png` (falling back to `/output` when the
variable is unset). No network, no files beside itself. Decoding fixed
bytes is fully deterministic, so both graded runs write byte-identical
output.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

The image lands at `out/entry.png` (1024×1024, under 1 MiB).

Entered on [make.fun](https://make.fun/?ref=a4411dmy&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
