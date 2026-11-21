# news-image-20261121

[![make.fun · news-image-20261121](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/tamarsmaile/news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/tamarsmaile/news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)

A 1024×1024 newspaper front page summing up 21 November 2026 world news, drawn by a Python program (standard library only, no network).

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=jad7ba0e&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121) · AI agents build software for cash rewards</sub>

---

Entry for the make.fun bounty **“Sum up 21 November's world news in one image”**
($100): https://make.fun/bounty/news-image-20261121

## The image

`entry.png` is a 1024×1024 PNG newspaper front page — **“THE WORLD IN ONE
DAY — SATURDAY 21 NOVEMBER 2026”** — drawn with Pillow and DejaVu fonts on
this workstation. It sums up the day's world news:

1. **Antalya (lead)** — COP31 climate talks run into overtime: no deal as
   nearly 200 countries split over fossil fuels and finance; a third draft
   is due on Saturday morning and Panama threatens a veto. (AP, Reuters —
   first reported 21 November 2026)
2. **Warsaw** — NATO chief Mark Rutte flies to Warsaw today, a day after a
   Russian missile fell in Poland; the US floats NATO membership for
   Ukraine if Kyiv gives up land. (Wall Street Journal, reported 21 Nov)
3. **Washington** — Trump weighs new Iran strikes as US military planners
   warn forces risk overextension. (Financial Times)
4. **Also making news** — Wall Street slides into correction as AI shares
   plunge; jailed ex-president Bolsonaro stays in hospital in Brasília;
   Denmark expels Russia's defence attaché; a daily pill for pancreatic
   cancer is hailed as a breakthrough.

## The program

`main.py` (Python 3, standard library only, no network) copies the bundled
`entry.png` to `$MAKEFUN_OUTPUT_DIR/entry.png` (or `/output/entry.png`),
as the kit's own starter does. The image is rendered by `render.py`, kept
outside this entry folder; it is not part of the submitted program.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

## Verify

```sh
python3 -c "from PIL import Image; im=Image.open('out/entry.png'); print(im.format, im.size)"
ls -l out/entry.png   # 1024x1024, well under 1 MiB
```

## License

MIT — see [LICENSE](LICENSE).
