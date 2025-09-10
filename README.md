# merklemap

[![basher install](https://www.basher.it/assets/logo/basher_install.svg)](https://www.basher.it/package/)

certificate transparency search for domains and subdomains

## install

```bash
basher install gnomegl/merklemap
```

## usage

```bash
merklemap example.com
```

discover subdomains via certificate transparency logs.

## options

- `-p, --page` - page number (default: 0)
- `-t, --type` - search type (wildcard/distance)
- `--csv` - csv output
- `-j, --json` - raw json

## requirements

- curl
- jq