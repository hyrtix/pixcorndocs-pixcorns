# 🌐 Configuration DNS - pixcorns.com

Guide pour configurer les enregistrements DNS de **pixcorns.com**.

## Enregistrements requis

| Type | Nom | Valeur | TTL |
|------|-----|--------|-----|
| A | @ | 92.222.229.242 | 600 |
| A | www | 92.222.229.242 | 600 |
| A | api | 92.222.229.242 | 600 |
| A | checkout | 92.222.229.242 | 600 |

## GoDaddy

1. My Products → pixcorns.com → **DNS**
2. Add → Type **A** pour chaque enregistrement
3. Name : @, www, api, checkout | Value : 92.222.229.242

## Cloudflare

**Proxy status** : **DNS only** (nuage gris) pour que Caddy gère le SSL.

## Vérification

```bash
dig pixcorns.com +short
# Doit retourner : 92.222.229.242
```
