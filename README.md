WIP

## Troubleshooting

If you get the following error when running `npm run package`:
```
Error: error:0308010C:digital envelope routines::unsupported
```

There is an issue here for this error: https://github.com/webpack/webpack/issues/14532

A workaround is to set the following environment variable:

```bash
export NODE_OPTIONS=--openssl-legacy-provider
```
