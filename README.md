# rulingyou.github.io

GitHub Pages site served at **https://rulinyu.com** (domain registered at Squarespace).

## DNS records (Squarespace → Domains → rulinyu.com → DNS)

Remove the default Squarespace records (the `@` A records pointing to 198.185.159.x / 198.49.23.x
and the `www` CNAME to `ext-sq.squarespace.com`), then add:

| Host | Type  | Data                  |
|------|-------|-----------------------|
| @    | A     | 185.199.108.153       |
| @    | A     | 185.199.109.153       |
| @    | A     | 185.199.110.153       |
| @    | A     | 185.199.111.153       |
| @    | AAAA  | 2606:50c0:8000::153   |
| @    | AAAA  | 2606:50c0:8001::153   |
| @    | AAAA  | 2606:50c0:8002::153   |
| @    | AAAA  | 2606:50c0:8003::153   |
| www  | CNAME | rulingyou.github.io   |

## Editing the site

All content is in `index.html`; styles are in `assets/style.css`. Search `index.html` for `[` to find
placeholders (prices, email, phone, location) that still need filling in.

## GitHub settings

Settings → Pages: deploy from the branch containing these files (root folder),
custom domain `rulinyu.com`, and tick **Enforce HTTPS** once the certificate is issued.
