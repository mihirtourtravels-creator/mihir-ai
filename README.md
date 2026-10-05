# M I H I R AI — Brand Video Studio MVP v0.7

## Commercial MVP
- 320+ ready-to-customize business promotional concepts
- Unified rule: **1 credit = 1 final AI creation** (image, video, poster, reel or promotional creative)
- Subscription plans: 1-day free trial, 1-day ₹100/2, 7-day ₹500/10, 15-day ₹1,000/20, 30-day ₹1,500/50, quarterly ₹4,000/150, half-yearly ₹7,000/300, yearly ₹11,000/1000
- Local persistent JSON backend for subscriptions, credits, creations, projects and consent-pending profiles, with subscription expiry enforcement and one-time free-trial protection
- Provider-neutral AI architecture for script, image/video, voice, avatar and rendering
- Multilingual-ready UI and template structure

## Run
Windows: double-click `run_mihir_ai.bat` and open http://127.0.0.1:8000
macOS/Linux: `./run_mihir_ai.sh`

## Important
This is a development MVP. Real AI video/avatar/voice rendering, payment gateway, cloud storage, authentication, moderation and identity verification still require production integrations. API secrets must remain server-side.


## v0.8 News Video Studio
- Short News mode: 15–60 seconds; user can paste only a script and create an AI-news-video job.
- Long News mode: 2–15 minutes for detailed bulletins.
- Presenter, voice, language and aspect-ratio controls.
- Human-review flag for publication; current/breaking news should be source-checked.
- News jobs consume the same unified 1-credit-per-final-creation rule.

## v0.9 local news renderer
POST `/api/render-news` with `{script, headline, mode, duration, human_review_required}`. It builds deterministic scenes and renders a test MP4 under `/renders/`. This is a technical renderer only; it does not claim to be an AI-generated presenter/video. Replace it with production provider adapters when credentials are configured.

## Direct Android APK
A GitHub Actions workflow is included at `.github/workflows/android-apk.yml`. Push this project to GitHub and the workflow will build `app-debug.apk` automatically. See `GITHUB_APK_BUILD.md`.
