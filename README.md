# dayz-integrations

This repository aims to provide all the integrations you might need for a DayZ server set-up. It includes the following:

- [Green Mountain Trader](https://wiki.mirasaki.dev/docs/gmt/overview) ([Trader](https://steamcommunity.com/sharedfiles/filedetails/?id=1590841260), [Trader Plus](https://steamcommunity.com/workshop/filedetails/?id=2458896948))
- [Expansion Market](https://wiki.mirasaki.dev/docs/expansion-market/overview)
- [Workshop Monitor](https://wm.mirasaki.dev/)
- [CFTools Discord Bot](https://github.com/Ariastarcos/cftools-discord-bot)

We use the following tools and framework to provide you with this functionality:

- Turborepo
- pnpm
- TypeScript
- ...

We implement the following APIs and services:

- Steam Query API
- CFTools Data API

## Web and UI/UX

### Adding components

To add components to your app, run the following command at the root of your `web` app:

```bash
pnpm dlx shadcn@latest add button -c apps/web
```

This will place the ui components in the `packages/ui/src/components` directory.

### Tailwind

Your `tailwind.config.ts` and `globals.css` are already set up to use the components from the `ui` package.

### Using components

To use the components in your app, import them from the `ui` package.

```tsx
import { Button } from "@workspace/ui/components/button"
```
