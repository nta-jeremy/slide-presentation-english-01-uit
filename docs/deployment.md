# Deployment

## Platform: Vercel

## Production URL

- https://slide-presentation-english-01-uit-group-02.vercel.app

## Verification

- Production alias verified: `HTTP 200` on 2026-05-27

## Deploy Command

```bash
vercel --prod
```

## Project Config

`vercel.json`:

```json
{
  "framework": null,
  "outputDirectory": "."
}
```

This project is deployed as a static HTML site from the repository root.

## Environment Variables

None required.

## Rollback

Use Vercel rollback with the target deployment URL:

```bash
vercel rollback <deployment-url>
```
