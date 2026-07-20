# PCB Company Profile

Static HTML/CSS company profile site for the Amazon Selling Partner API Solution Provider Portal review. The site explains that PCB operates its own Amazon.co.jp sales business and uses SP-API for internal operational efficiency with ReadOnly access.

## Public URL

https://takeijp-site.github.io/pcb-company-profile/

## Confirmed business information

- Legal name: PCB
- Representative: &#x8449;&#x888B; &#x96C4;&#x4E09;
- Address: &#x3012;405-0074 &#x5C71;&#x68A8;&#x770C;&#x7B1B;&#x5439;&#x5E02;&#x4E00;&#x5BAE;&#x753A;&#x56FD;&#x5206;927
- Phone: `090-8141-6245`
- Telephone link: `tel:09081416245`
- Email: `takeijpdev@gmail.com`
- Mail link: `mailto:takeijpdev@gmail.com`

The site does not claim Amazon partnership, certification, or official status. It does not use an Amazon logo, advertising, social media, cookies, external fonts, or JavaScript.

## Directory

```text
.
|-- 404.html
|-- favicon.svg
|-- index.html
|-- privacy.html
|-- robots.txt
|-- site.webmanifest
|-- sitemap.xml
|-- style.css
`-- SHA256SUMS.txt
```

## GitHub Pages publication

1. Copy the contents of this directory to the root of the GitHub repository.
2. Open GitHub **Settings > Pages**.
3. Select **Deploy from a branch**, choose the publication branch and `/ (root)`.
4. Open the issued URL and check the home page, privacy page, 404 page, phone link, and email link.
5. When the public URL is known, add the real home and privacy URLs to `sitemap.xml` and optionally add the sitemap URL to `robots.txt`.
6. For a custom domain, update the GitHub Pages custom-domain setting and DNS, then update the sitemap URLs.

## Local check

```powershell
py -m http.server 8080
```

Open `http://localhost:8080/` in a browser. The site is static and requires no build step.

## Hashes

`SHA256SUMS.txt` contains SHA-256 hashes for every deliverable except itself. Regenerate it after any file change:

```powershell
Get-ChildItem -File | Where-Object { $_.Name -ne 'SHA256SUMS.txt' } | Sort-Object Name | Get-FileHash -Algorithm SHA256 | ForEach-Object { "$($_.Hash.ToLower())  $($_.Path | Split-Path -Leaf)" } | Set-Content -Encoding ascii SHA256SUMS.txt
```

