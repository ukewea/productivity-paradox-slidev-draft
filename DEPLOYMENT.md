# Deployment

This deck deploys as a static Slidev site to Cloudflare Pages. GitHub Actions builds the deck, then uploads the generated `dist/` directory with Wrangler.

## Architecture

```text
GitHub repo
  -> GitHub Actions workflow
  -> npm ci
  -> npm run build
  -> dist/
  -> Cloudflare Pages
  -> https://productivity-paradox-slidev-draft.pages.dev
```

The workflow lives at:

```text
.github/workflows/deploy-cloudflare-pages.yml
```

## One-Time Setup

### 1. Create the Cloudflare Pages project

Install/use Wrangler, log in, then create the Pages project:

```bash
npx wrangler login
npx wrangler pages project create productivity-paradox-slidev-draft --production-branch main
```

If you use a different Cloudflare project name, update `CLOUDFLARE_PROJECT_NAME` in `.github/workflows/deploy-cloudflare-pages.yml`.

### 2. Create a Cloudflare API token

In Cloudflare:

```text
My Profile -> API Tokens -> Create Token -> Custom Token
```

Required permission:

```text
Account / Cloudflare Pages / Edit
```

Also copy the Cloudflare account ID from the dashboard.

### 3. Add GitHub Actions secrets

In GitHub:

```text
Repo -> Settings -> Secrets and variables -> Actions -> New repository secret
```

Add these repository secrets:

```text
CLOUDFLARE_ACCOUNT_ID = Cloudflare account ID
CLOUDFLARE_API_TOKEN  = Cloudflare API token
```

`GITHUB_TOKEN` does not need to be created manually. GitHub provides it automatically inside Actions.

## Deploy

Deploy happens automatically on pushes to `main`:

```bash
git push origin main
```

You can also deploy manually:

```text
GitHub repo -> Actions -> Deploy slides to Cloudflare Pages -> Run workflow
```

## Local Check Before Pushing

Run:

```bash
npm ci
npm run build
```

The build output should appear in `dist/`. The `dist/` directory is generated output and is ignored by git.

## Notes

- This project currently uses Slidev `0.50.0`.
- `slidev build` works for this repo.
- The newer `--without-notes` option mentioned in current Slidev docs is not supported by this installed version.
- Because the deployed site is public, do not put private/internal-only material in `slides.md` or assets.

## Official References

- Cloudflare Pages CI with Wrangler: https://developers.cloudflare.com/pages/how-to/use-direct-upload-with-continuous-integration/
- Wrangler Pages commands: https://developers.cloudflare.com/workers/wrangler/commands/pages/
- Cloudflare API tokens: https://developers.cloudflare.com/fundamentals/api/get-started/create-token/
- Cloudflare account ID: https://developers.cloudflare.com/fundamentals/account/find-account-and-zone-ids/
- GitHub Actions secrets: https://docs.github.com/en/actions/how-tos/write-workflows/choose-what-workflows-do/use-secrets
