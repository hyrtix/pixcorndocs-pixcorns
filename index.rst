Pixcorns Payment Gateway API Documentation (pixcorns.com)
=========================================================

Welcome to the Pixcorns Payment Gateway API documentation for **pixcorns.com**. This documentation will help you integrate Pixcorns into your application to process high-risk payments with instant USDC settlements.

Getting Started
---------------

Pixcorns is a high-ticket payment gateway designed for enterprise businesses processing $10M+ annually. It provides instant USDC settlements on Polygon network with zero KYC requirements.

How It Works
-----------

1. **Account Creation**: The Pixcorns admin will create your merchant account and provide you with:
   - Your unique API key
   - Your merchant ID (`public_id`)
   - Your USDC wallet address for receiving payments
   - Your commission rate (if applicable)

2. **API Integration**: Use your API key to authenticate all API requests

3. **Payment Processing**: Create payment links and redirect customers to the Pixcorns checkout page

4. **Webhooks**: Receive instant notifications when payments are completed

Quick Start
-----------

Once you receive your API key from the Pixcorns admin, you can start processing payments immediately:

.. code-block:: bash

   curl -X POST https://pixcorns.com/payments/api/create/ \
     -H "Content-Type: application/json" \
     -H "X-API-Key: YOUR_API_KEY_HERE" \
     -d '{
       "amount": 100.00,
       "currency": "EUR",
       "customer_email": "customer@example.com"
     }'

Configuration DNS
-----------------

See `DNS_SETUP.md` for DNS configuration (pixcorns.com → 92.222.229.242).

Contents
--------

.. toctree::
   :maxdepth: 2

   authentication
   payment_api
   webhooks
   error_handling
