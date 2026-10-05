# backlog.md — Odoo TR E-Ticaret Fikir Havuzu

README'deki modül planı (öncelik sırası önerisi):

1. `payment_iyzico` → 2. `delivery_yurtici` → 3. `website_sale_rest_api` + `website_sale_jwt_auth` → 4. `payment_paytr` → 5. diğer kargolar (`delivery_aras`, `delivery_mng`, `delivery_ptt`) → 6. SaaS modülleri (`saas_subscription`, `saas_quota`, `saas_api_key`, `saas_billing`) → 7. `payment_stripe_tr`.

Ek fikirler:
- e-Arşiv/e-Fatura bağlantısı (`l10n_tr_sovos_efatura` ile sipariş → fatura).
- Pazaryeri entegrasyonları (Trendyol, Hepsiburada) — stok/sipariş senkronu.
- n8n ile sipariş bildirimleri (WhatsApp/e-posta) — `n8nOdoo` deneyimi.

## Ekleme Şablonu

```markdown
### Başlık
- **Kategori:** yeni modül / iyileştirme / araştırma
- **Neden:** kısa gerekçe
- **Notlar:** Odoo sürümü, bağımlılıklar, riskler
```
