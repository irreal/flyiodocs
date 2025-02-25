---
title: Dockerfiles
layout: framework_docs
objective: Get started by generating a Dockerfile used to build and deploy your application.
order: 0
---

The recommended way to deploy Bun, Deno, and Node.js applications is via
[Dockerfiles](https://docs.docker.com/engine/reference/builder/).  You can
provided your own Dockerfile or you can let fly.io's
[dockerfile generator](https://github.com/fly-apps/dockerfile-node#overview)
produce one for you.

Launching applications on Fly can be as simple as running:

```cmd
fly launch
```

In most cases you won't ever need to edit this Dockerfile directly.  Instead you will be
able to use one or more of the may [options](https://github.com/fly-apps/dockerfile-node#options)
to make changes.  For example:

```cmd
npx dockerfile --add=dnsutils
```