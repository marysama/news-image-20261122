# Sum up 22 November's world news in one image

Entry for [make.fun bounty `news-image-20261122`](https://make.fun/bounty/news-image-20261122)
— $100, 50 places paid, deadline Tue 24 Nov 2026 07:00 WIB (00:00 UTC).

## What it is

A newspaper front page, 1024×1024 PNG, summing up Sunday 22 November 2026:

- **Lead — Gulf tensions:** at least two tankers struck near the Strait of
  Hormuz; Bahrain reported an Iranian attack on a civilian industrial
  facility in Sitra (fire, two injured); Iran's foreign minister said
  reopening the strait is not difficult if the U.S. accepts Tehran's
  conditions.
- **Climate — COP31:** the summit in Antalya ended with no agreement after
  ~200 countries failed to agree on fossil fuels or finance; the EU,
  Britain and allies rejected the final draft.
- **Russia–Ukraine war:** suspected Ukrainian sea drones struck a Russian
  naval vessel docked at Benghazi Naval Base, Libya.
- **World Court:** the ICJ ruled Myanmar committed genocide against the
  Rohingya minority.
- **Indonesia:** a candy-factory fire in Cikande, Banten killed at least
  three people, with 36 missing.
- **Mexico:** troops captured drug lord 'El Chapo Isidro' in Sinaloa;
  11 people died in the firefight.
- **Footer:** UK–EU post-Brexit trade & travel deals; India declared
  720/9 vs New Zealand, a 352-run lead.

Sources: Open Chronicle Global News Brief 22 Nov 2026, Seven Lights,
KPFA Pacifica Evening News 22 Nov 2026, Reuters/AP headlines.

## How it runs

`main.py` (Python 3.13, standard library only) copies the bundled
`entry.png` to `/output/entry.png`. The brief allows the simplest program
to copy an image the repository holds. No network, no clock, no randomness:
two runs write identical bytes.

```sh
python3 main.py   # writes /output/entry.png
```

The image was drawn at build time by `generate.py` (Pillow, DejaVu fonts)
in the build workspace; the submitted repository holds only `main.py`,
`entry.png`, `LICENSE` and this README.

## Requirements check

- 1024×1024 PNG, 145,493 bytes (limit 1 MiB) ✓
- Deterministic: two runs byte-identical (SHA-256 verified) ✓
- No network at run time ✓
