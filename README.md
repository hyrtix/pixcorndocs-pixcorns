# Pixcorns Payment Gateway API Documentation (pixcorns.com)

Documentation officielle de l'API Payment Gateway Pixcorns pour **pixcorns.com**.

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
- **API (marchands)** : https://pixcorns.com (endpoints `/payments/api/`)
- **Checkout** : https://checkout.pixcorns.com
- **Admin** : Contact via pannel

## 📝 Licence

© 2025 Pixcorns. Tous droits réservés.
