# onetimesecret

![Version: 0.1.0-RC3](https://img.shields.io/badge/Version-0.1.0--RC3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.17.3](https://img.shields.io/badge/AppVersion-v0.17.3-informational?style=flat-square)

A Helm chart for OnetimeSecret

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://charts.bitnami.com/bitnami | redis | 20.1.5 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `true` |  |
| ingress.hosts[0].host | string | `"onetimesecret.example.com"` |  |
| ingress.hosts[0].paths[0] | string | `"/"` |  |
| ingress.tls | list | `[]` |  |
| onetimesecret.env.COLONEL | string | `"admin@example.com"` |  |
| onetimesecret.env.FROM_EMAIL | string | `"no-reply@example.com"` |  |
| onetimesecret.env.SMTP_HOST | string | `"smtp.example.com"` |  |
| onetimesecret.env.SMTP_PASSWORD | string | `"password"` |  |
| onetimesecret.env.SMTP_PORT | string | `"587"` |  |
| onetimesecret.env.SMTP_USERNAME | string | `"username"` |  |
| onetimesecret.env.SSL | string | `"true"` |  |
| onetimesecret.env.TO_EMAIL | string | `"no-reply@example.com"` |  |
| onetimesecret.image.registry | string | `"docker.io"` |  |
| onetimesecret.image.repository | string | `"onetimesecret/onetimesecret"` |  |
| onetimesecret.image.tag | string | `""` |  |
| onetimesecret.service.type | string | `"ClusterIP"` |  |
| redis.architecture | string | `"standalone"` |  |
| redis.auth.enabled | bool | `false` |  |
| redis.enabled | bool | `true` |  |
| redis.master.persistence.enabled | bool | `true` |  |
| redis.master.persistence.size | string | `"1Gi"` |  |
