# Heroku Buildpack for Deno

This is a Heroku buildpack for Deno apps.

Web processes must bind to `$PORT`, and only the HTTP protocol is permitted for incoming connections.

## Detection

This buildpack requires a `main.ts` at the root of the build directory.

Dependencies of `main.ts` will be cached.

## Specify a Deno Runtime

To specify your Deno version, you also need a `.deno-version` file - unless you are using the latest Deno runtime version.
```
$ cat .deno-version
v0.41.0
```
