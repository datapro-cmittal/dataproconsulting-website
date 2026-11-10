# Datapro Consulting Limited — GitHub Pages

## Publish
1. Sign in to GitHub and create a **public** repository named `dataproconsulting-website`.
2. Upload `index.html` and `CNAME` from this folder to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main`, folder `/(root)`, then Save.
6. GitHub will publish the site at `https://YOUR-USERNAME.github.io/dataproconsulting-website/`.

## Connect the custom domain
In **Settings → Pages → Custom domain**, enter `dataproconsulting.co.uk` and save.
At Namecheap → Domain List → Manage → Advanced DNS, add/update only the website records:

- A, Host `@`, Value `185.199.108.153`
- A, Host `@`, Value `185.199.109.153`
- A, Host `@`, Value `185.199.110.153`
- A, Host `@`, Value `185.199.111.153`
- CNAME, Host `www`, Value `YOUR-USERNAME.github.io`

Replace `YOUR-USERNAME` with your actual GitHub username (no repository name in this CNAME target).

**Important:** Do not delete or change Microsoft 365 MX, TXT, or CNAME records used for email (including MX, SPF, autodiscover, DKIM and DMARC records). Add the website records alongside them. If an `@` A record already exists for another website, check before replacing it.

After DNS propagates, return to Settings → Pages and enable **Enforce HTTPS** when GitHub makes it available.
