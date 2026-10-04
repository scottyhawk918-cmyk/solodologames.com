# solodologames.com

The SoloDolo Games website: one page (`index.html`) about Off Grid'n, with the trailer, screenshots and a press kit.
It's hosted free on **GitHub Pages**; the domain (solodologames.com) is registered at **GoDaddy**.

## Changing the site

1. Edit `index.html` (or swap pictures in `img/shots/`).
2. Commit and push. GitHub puts the new version live in a minute or two.

## How the domain points here (one-time setup, already done once it works)

In GoDaddy: **My Products → solodologames.com → DNS**, then:

| Type  | Name | Value                              |
|-------|------|------------------------------------|
| A     | @    | 185.199.108.153                    |
| A     | @    | 185.199.109.153                    |
| A     | @    | 185.199.110.153                    |
| A     | @    | 185.199.111.153                    |
| CNAME | www  | scottyhawk918-cmyk.github.io       |

Delete any other **A** record for `@` (GoDaddy's "Parked" one) and any old `www` record first.
On GitHub: the repo's **Settings → Pages**: custom domain `solodologames.com`, then tick **Enforce HTTPS** once it's offered.
The `CNAME` file in this folder tells GitHub which domain the site is for: keep it.

## What's where

- `img/shots/`: screenshots (`name.jpg` is 1600 px wide, `name_sm.jpg` is the small one shown on the page)
- `img/share.jpg`: the picture shown when someone shares a link to the site
- `video/`: the trailer and the SoloDolo logo animation (made by `tools/make_trailer.py` in the game repo)
- `presskit.zip`: logos, screenshots and a fact sheet for press
