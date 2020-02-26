# proxify now

As long as Now CLI does not support being run behind a proxy (see https://github.com/zeit/now/issues/255) you can do so with this small wrapper.

# Usage

Install proxify-now:

```
npm i -g now global-agent proxify-now
```

Set your http_proxy, https_proxy and no_proxy environment variables.

Start using Now CLI with support for http_proxy, https_proxy and no_proxy:

```
pnow <any Now CLI commands>
```

# How does it work?

proxify-now runs Now CLI with ```global-agent``` preloaded. ```global-agent``` adds proxy support to any http agent running in the process.
