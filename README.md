# Firefox Policies

A simple Firefox config to disable unwanted features.

## Install

```bash
sh -c 'tmp="$(mktemp -d)" || exit 1; git clone --depth 1 https://github.com/dumbovita/policies "$tmp" && sudo mkdir -p /etc/firefox/policies && sudo install -m 644 "$tmp/policies.json" /etc/firefox/policies/policies.json; status=$?; rm -rf "$tmp"; exit $status'
```

## Check

Restart Firefox and open:

```text
about:policies
```

## Location

The policy file is installed to (on linux):

```text
/etc/firefox/policies/policies.json
```
