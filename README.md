# CART3R Forge AI — browser MVP

## Start on iPad
1. Extract the ZIP using Files.
2. Open `index.html` in a browser. If iPadOS won't open it as a webpage, host the file using GitHub Pages (below).
3. The starter strategy prototype is playable without an AI key.
4. Create an OpenRouter account at https://openrouter.ai/ and obtain an API key from https://openrouter.ai/settings/keys. Check the currently available free model options at https://openrouter.ai/models?max_price=0. The default `openrouter/free` router may be supported, but free access, rate limits and routing can change.
5. Paste the key into the AI connection field. The key stays in memory for this tab and is not intentionally persisted. It is sent directly from your browser to OpenRouter for inference. Do not paste other people's keys.
6. Describe a small feature, click Generate code, review the proposal, click Apply proposal, and Refresh preview. Export project JSON regularly.

## Publish for free using GitHub Pages
1. Sign in at https://github.com/ and create a **public** repository, e.g. `cart3r-forge`.
2. Upload `index.html` to the repository root.
3. In repository Settings → Pages → Build and deployment, choose Deploy from a branch → `main` → `/ (root)` → Save.
4. Open the Pages URL displayed by GitHub when published. GitHub Pages hosting is public; never put private API keys into the source file or repository.
5. The app works as a static site. Your browser's local project storage does **not** automatically sync between devices or browsers.

## Limitations
- This is an MVP, not a fully autonomous multi-file agent. Each AI request proposes a complete replacement for one file; you approve it.
- OpenRouter free-tier quotas and model availability can change. Browser-to-provider requests can fail due to CORS, provider restrictions, or account limits.
- The game is a small six-country economic/turn prototype, not an actual geographical map or a full HOI4 clone.
- Browser localStorage is not durable backup; export JSON after every significant change.
- AI-generated code is untrusted. Preview runs in a sandboxed iframe without same-origin access, but still review source before downloading or publishing.
- There is no server, automatic GitHub commits, persistent agent memory, multi-file patching or automatic tests in this version.
- Do not upload proprietary Hearts of Iron IV assets or source code.
