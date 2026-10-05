# npub.nfunc.xyz

> Nostr profile viewer.

**Live**: <https://npub.nfunc.xyz>

## Stack

- [Vite](https://vitejs.dev/) + React 18 + TypeScript
- Tailwind CSS
- lucide-react

## Nostr

- **Login**: NIP-07 (browser extension) + NIP-55 (Amber callback URI)
- `kind:0` — profile metadata
- `kind:1` — short notes

Reads from `wss://relay.nfunc.xyz`.

## Develop

```bash
npm install
npm run dev
```

## Build + deploy

```bash
./deploy.sh
```

Builds, rsyncs `dist/` to the deploy host and checks the live site serves the
new build.

## The three forks

npub is published three times from three repos that differ only in palette,
hostnames and the relay they read: the coral one, the emerald one and this
monochrome one, which is the nfunc.xyz member.

---

_Sister repos: <https://github.com/macos-node/npub.upleb.uk> · <https://github.com/adjmx/npub.fizx.uk>_
