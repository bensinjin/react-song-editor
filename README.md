# React-Song-Editor

Playing with publishing the song editor component from https://ramblepad.app.

# Development

WIP.

## Local development

1. Setup a monorepo with a couple workspaces, in `package.json`:

```
{
  "name": "react-song-editor-dev",
  "private": true,
  "workspaces": ["packages/*"]
}
```

1. Clone `react-song-editor` and run: `npm run dev` from inside the package to watch for changes.
1. Create a test app (see below to use vite) and run the dev server.
1. `import { SongEditor } from "react-song-editor";` into your test app.

## Testing a release

From `react-song-editor`:

1. `npm run build`
1. `yalc publish`

Create test app and install package:

1. `npm create vite@latest react-song-editor-test -- --template react-ts`
1. `yalc add react-song-editor`
1. `npm i`
