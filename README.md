# lldap

> Click To Deploy lldap — Lightweight LDAP Server with a friendly web UI

[![Sync](https://github.com/opensaasapps/lldap/actions/workflows/sync.yml/badge.svg)](https://github.com/opensaasapps/lldap/actions/workflows/sync.yml) [![Docker](https://github.com/opensaasapps/lldap/actions/workflows/docker.yml/badge.svg)](https://github.com/opensaasapps/lldap/actions/workflows/docker.yml) [![Docker Pulls](https://img.shields.io/docker/pulls/thefractionalpm/lldap)](https://hub.docker.com/r/thefractionalpm/lldap)

Upstream: [lldap/lldap](https://github.com/lldap/lldap) · Auto-synced daily

---

## One-Command Deploy

```bash
cp .env.example .env && nano .env
docker compose up -d
```

## Coolify / Dokploy

1. New service → **Docker Compose**
2. Paste `docker-compose.yml`
3. Set env vars in UI
4. Deploy

## Environment Variables

| Variable | Required | Description |
|---|---|---|
| `LLDAP_JWT_SECRET` | ✅ | |
| `LLDAP_KEY_SEED` | ✅ | |
| `LLDAP_LDAP_BASE_DN` | ⚪ | |
| `LLDAP_LDAP_USER_PASS` | ✅ | |
| `LLDAP_LDAP_USER_EMAIL` | ⚪ | |
| `LLDAP_DATABASE_URL` | ⚪ | |
| `LLDAP_HTTP_URL` | ⚪ | |
| `LLDAP_SMTP_OPTIONS__ENABLE_PASSWORD_RESET` | ⚪ | |
| `LLDAP_SMTP_OPTIONS__SERVER` | ✅ | |
| `LLDAP_SMTP_OPTIONS__PORT` | ⚪ | |
| `LLDAP_SMTP_OPTIONS__TLS_REQUIRED` | ⚪ | |
| `LLDAP_SMTP_OPTIONS__USER` | ✅ | |
| `LLDAP_SMTP_OPTIONS__PASSWORD` | ✅ | |
| `LLDAP_SMTP_OPTIONS__FROM` | ⚪ | |

## Image

```
docker pull lldap/lldap:stable
docker pull thefractionalpm/lldap:latest
```

## Ports

| Port | Service |
|---|---|
| `17170` | Main app |

---

*Part of the [OpenSaaSApps](https://github.com/opensaasapps) Click-To-Deploy collection.*
