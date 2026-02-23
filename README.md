# Pixcorn Payment Gateway API Documentation (pixcorns.com)

Documentation officielle de l'API Payment Gateway Pixcorn pour **pixcorns.com**.

## 📚 Documentation

La documentation complète est disponible sur : **[docs.pixcorns.com](https://pixcorns-api-docs.readthedocs.io/)** (ou hébergée localement)

## 🚀 Quick Start

```bash
curl -X POST https://pixcorns.com/payments/api/create/ \
  -H "Content-Type: application/json" \
  -H "X-API-Key: YOUR_API_KEY_HERE" \
  -d '{
    "amount": 100.00,
    "currency": "EUR",
    "customer_email": "customer@example.com"
  }'
```

## 🌐 Configuration DNS (pixcorns.com)

| Type | Nom | Valeur |
|------|-----|--------|
| A | @ | 92.222.229.242 |
| A | www | 92.222.229.242 |
| A | api | 92.222.229.242 |
| A | checkout | 92.222.229.242 |

Voir `DNS_SETUP.md` pour les instructions détaillées par registrar (GoDaddy, Cloudflare, etc.).

## 📖 Contenu

- **Authentication** : Authentification par clé API
- **Payment API** : Création et gestion des paiements
- **Webhooks** : Notifications de paiement
- **Error Handling** : Codes d'erreur et réponses

## 🔧 Build local

```bash
pip install -r requirements.txt
make html
```

La documentation sera générée dans `_build/html/`.

## 🌐 URLs

- **Site principal** : https://pixcorns.com
- **API** : https://api.pixcorns.com
- **Checkout** : https://checkout.pixcorns.com
- **Admin** : https://pixcorns.com/admin/

## 📝 Licence

© 2025 Pixcorn Digital Solutions. Tous droits réservés.
