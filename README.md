# StashSphere Frontend

⚠️⚠️⚠️

THE DEVELOPMENT HAS MOVED TO [github.com/stashsphere/stashsphere](https://github.com/stashsphere/stashsphere/tree/main/frontend).
THIS REPOSITORY IS NOW ARCHIVED AND READ-ONLY. IT WILL BE DELETED ON 2026/02/01.

⚠️⚠️⚠️

This is the frontend of stashsphere built using React, Typescript and Vite.

## Config

The application is configured using a simple config object. It configures
first and foremost the API base url of the backend.
In production mode the config is fetched relative to the frontend location,
in development mode the config is static, see `src/config/config.development.ts`.

## Nix

The frontend can be built using the provided nix flake. This also allows to
generate the config on-the-fly, see the `apiHost` argument.

Build:

```
nix build .#frontend
```

## License

AGPL v3
