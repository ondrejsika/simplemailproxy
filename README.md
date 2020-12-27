# simplemailproxy - helm chart

    2020 Ondrej Sika <ondrej@ondrejsika.com>
    https://github.com/ondrejsika/simplemailproxy-helm

## Usage

Add repo

```
helm repo add ondrejsika https://helm.oxs.cz
```

Install

```
helm upgrade --install \
  <name> ondrejsika/simplemailproxy \
  --set domainHostPortList=<list of domain:host:port>
  --set smtpNodePort=<port>
```

## Parameters

### Required

- `domainHostPortList` - List of `domain:host:port` config (example: `foo.com:foo-smtp:25`)

### Optional

- `smtpNodePort`
