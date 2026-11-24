# Mastery legacy redirect

Static hosting for `mastery.aiaimastermind.com` on GitHub Pages.

`index.html` and `404.html` are identical so old deep links execute the same redirect. Ordinary paths, query strings, invitation tokens and fragments are preserved. Previous-provider authentication callbacks deliberately discard stale credentials and go to `https://mastery.insight2impactai.com/login?error=access_denied`, matching legacy release `47ff47b`.

The only preview-specific rule removes `/mastery-legacy-redirect` on `philgoodvibe.github.io`. The custom hostname preserves the full path.

No application, analytics, credentials, database access or build dependencies are included.
