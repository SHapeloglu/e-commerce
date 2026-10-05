# architect.md — Odoo TR E-Ticaret Hedef Mimarisi

Kod henüz yok; bu dosya README'deki hedef mimariyi ve modül planını özetler.

```
Next.js / React frontend (sepet, sipariş, kullanıcı paneli)
        │ REST (website_sale_rest_api + website_sale_jwt_auth) / JSON-RPC
        ▼
Odoo Community 18.0
 ├─ OCA: e-commerce, sale-workflow, stock-logistics, (product-attribute, web…)
 └─ Bu repo (planlanan):
     ├─ Ödeme:  payment_iyzico (3D Secure, webhook, iade), payment_paytr, payment_stripe_tr
     ├─ Kargo:  delivery_yurtici, delivery_aras, delivery_mng, delivery_ptt (barkod, etiket, takip)
     ├─ SaaS:   saas_subscription (free/pro/enterprise), saas_quota, saas_api_key, saas_billing
     └─ API:    website_sale_rest_api, website_sale_jwt_auth
```

## Kurulum Akışı (README "Hızlı Başlangıç")

1. OCB 18.0 klonla.
2. `OCA/e-commerce` (18.0) ve bu repo `addons/` altına.
3. `odoo.conf` → `addons_path`.
4. `./odoo-bin -d <db> -i website_sale_product_assortment,website_sale_stock_available,payment_iyzico`.

## Mimari Kararlar

- **OCA önce, custom sonra**: ihtiyacın ~%70'i OCA ile; sadece Türkiye'ye özgü boşluklar (yerel ödeme/kargo) ve SaaS/headless katmanı yazılacak.
- **Headless seçeneği**: Odoo website yerine ayrı frontend; Odoo backend/ERP olarak kalır.
