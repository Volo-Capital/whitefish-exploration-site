# Whitefish Exploration landing page

Static one-page website prepared for free hosting on GitHub Pages.

## Publish with GitHub Pages

1. Create a public repository named `whitefish-exploration-site` under the `Volo-Capital` organization.
2. Upload every file from this folder to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select **main**, choose **/(root)**, and click **Save**.
6. Under **Custom domain**, enter `whitefishexploration.com` and click **Save**.
7. After DNS resolves, enable **Enforce HTTPS**.

## GoDaddy DNS

Delete or replace only the existing website **A record** named `@` that currently says `WebsiteBuilder Site`. Add these four A records:

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |

Edit the existing `www` CNAME:

| Type | Name | Value |
| --- | --- | --- |
| CNAME | www | volo-capital.github.io |

Do not alter the Lark MX, SPF, verification, or other email records.

## Replit editing

Replit can be used as the editor without hosting the site there. Import this GitHub repository into Replit, edit the files, preview the page, then commit and push changes back to GitHub. GitHub Pages republishes after each push.

## Search indexing

After the site is live, add `whitefishexploration.com` to Google Search Console, submit `https://whitefishexploration.com/sitemap.xml`, and request indexing for the homepage.
