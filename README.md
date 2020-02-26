# proxify now

As long as Now CLI does not support being run behind a proxy (see https://github.com/zeit/now/issues/255) you can do so with this small wrapper.

# Usage

To install proxify-now run this command:

```
npm i -g now global-agent proxify-now
```

**Set your http_proxy, https_proxy and no_proxy environment variables.**

To start using Now CLI with support for http_proxy, https_proxy and no_proxy run this command:

```
pnow <any Now CLI commands>
```

# How does it work?

Proxify now uses global-agent as a wrapper to run Now CLI. Global-agent adds proxy support to any http agent running within the wrapped process.
