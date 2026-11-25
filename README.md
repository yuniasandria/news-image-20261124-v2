# News Image — Tuesday 24 November 2026

One image summing up the full day's world news: **36 dated stories,
10 regions, every one checked** in a named outlet.

- Lead: US jury convicts Huawei on 10 of 12 counts (trade secrets and
  bank fraud; acquitted of racketeering).
- 35 more cards: Ukraine strikes Russian ships in two seas, IRGC attacks
  in the Strait of Hormuz, ICJ finds Myanmar guilty of Rohingya genocide,
  COP31 ends with no deal, Huang returns as Nvidia CEO, Senegal regain
  the AFCON title, and 29 more — each tagged with its region and outlet.

## How it runs

`main.py` is pure Python 3.13 standard library: it draws the front page
on a 1024×1024 canvas with a bitmap font embedded as data (glyphs
rendered at build time from DejaVu Sans) and writes its own PNG with
`zlib` + `struct`. No third-party imports, no network.

```
python3 main.py   # writes /output/entry.png (or $MAKEFUN_OUTPUT_DIR/entry.png)
```

Entry for the make.fun competition
[`news-image-20261124`](https://make.fun/c/news-image-20261124).
