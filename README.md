# ValuVale — public site

Static pages served by GitHub Pages. No build step, no dependencies.

| Path | Purpose |
|---|---|
| `privacy/index.html` | Privacy policy, TR + EN toggle. This URL goes into App Store Connect. |
| `index.html` | Root redirect to the privacy page (landing page can replace it later). |

## Publish (one time)

1. Create a **public** repo `valuvale-site` under your GitHub account.
2. Copy the contents of this folder to the repo root and push.
3. Repo → Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)` → Save.
4. After ~1 minute the policy is live at
   `https://<user>.github.io/valuvale-site/privacy/`
   Use that exact URL in App Store Connect → App Privacy → Privacy Policy URL.

## Keep in sync

The in-app policy (`valuvale/Views/Settings/PrivacyPolicyView.swift`) and this page carry the same sections and the same "Last updated" date. Change both together.

## Custom domain later

When `valuvale.app` (or similar) is bought: add a `CNAME` file containing the domain, point the domain's DNS at GitHub Pages, and update the URL in App Store Connect. Nothing else changes.
