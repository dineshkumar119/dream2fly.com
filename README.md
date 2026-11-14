# DreamToFly Aviation Services (dreamtofly.com)

Static website: MRO overview, operations, departments and regulators (DGCA, EASA, FAA, ICAO).
No build step. `index.html` is the whole site.

## Publish on GitHub Pages
1. Create a repository on GitHub (e.g. `dreamtofly`) and push these files to the `main` branch.
2. Repository > Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Settings > Pages > Custom domain: `dreamtofly.com` (the `CNAME` file already holds it). Tick "Enforce HTTPS" when it is available.
4. At your domain registrar, add DNS records:
   - `A`  `@`  185.199.108.153
   - `A`  `@`  185.199.109.153
   - `A`  `@`  185.199.110.153
   - `A`  `@`  185.199.111.153
   - `CNAME`  `www`  `YOUR-GITHUB-USERNAME.github.io`

## Show up in Google
1. Open Google Search Console and add `https://dreamtofly.com` as a property; verify it (DNS TXT record).
2. Submit `https://dreamtofly.com/sitemap.xml`.
3. Use "URL inspection" > "Request indexing" for the home page.
