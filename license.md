
---

## Deploy checklist

1. `npm install && npm run vendor` — populates `baremux/` and `epoxy/`
2. Push everything to `absurdaltacc.github.io` `main`
3. GitHub Pages → Source: Deploy from branch → `main` / root
4. Open `https://absurdaltacc.github.io/`
5. DevTools → Console should show three `[absent]` logs
6. Type `google.com` → should render

If it still says "refused to connect" after this, open DevTools → Network, filter `scramjet`, and tell me what URL shows up. That tells us instantly whether the SW is intercepting or the frame is loading directly.