# 🛒 Odoo E-Ticaret Kurulum Rehberi (OCA Free Modüller)

> Bu rehber, **Odoo Community + OCA ücretsiz modülleri** kullanarak sıfırdan çalışan bir e-ticaret sistemi kurmanıza yardımcı olur.  
> Eksik kalan kritik parçalar için **bu repodaki custom modüller** geliştirilmiştir.

---

## 📦 Adım 1 — Temel Kurulum

Önce Odoo Community Edition'ı kurun:

```bash
# Odoo 17.0 veya 18.0 (Community)
git clone https://github.com/OCA/OCB.git --branch 18.0
```

---

## ✅ Adım 2 — OCA Ücretsiz Modüller (Kurmanız Gerekenler)

Aşağıdaki modülleri kurarak e-ticaret sisteminizin **%70'ini hazır** hale getirebilirsiniz.

### 🏪 Ürün & Katalog

| Modül | Repo | Ne Sağlar |
|---|---|---|
| `product_template_multi_link` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Ürün çoklu bağlantı yönetimi |
| `product_variant_multi_link` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Varyant bazlı çoklu bağlantı |
| `website_sale_product_brand` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Mağazada marka filtreleme |
| `website_sale_product_sort` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Varsayılan sıralama kriteri |
| `website_sale_product_assortment` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Ürün koleksiyonu ile vitrin yönetimi |
| `website_sale_product_minimal_price` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Varyantlar için minimum fiyat gösterimi |
| `website_sale_product_description` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Özel e-ticaret ürün açıklaması |
| `website_sale_product_detail_attribute_image` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Ürün sayfasında özellik görseli |
| `website_sale_barcode_search` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Barkod ile ürün arama |
| `website_sale_hide_empty_category` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Boş kategorileri gizle |
| `website_sale_hide_price` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Fiyatı gizle (B2B için) |
| `website_snippet_product_category` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Sayfaya kategori widget'ı ekle |

### 📦 Stok & Sipariş

| Modül | Repo | Ne Sağlar |
|---|---|---|
| `website_sale_stock_available` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Mağazada stok miktarı gösterimi |
| `website_sale_stock_list_preview` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Ürün kartında stok önizleme |
| `website_sale_stock_provisioning_date` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Tahmini temin tarihi gösterimi |
| `website_sale_cart_expire` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Hareketsiz sepeti otomatik iptal |
| `website_sale_empty_cart` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Sepeti tamamen temizle butonu |
| `website_sale_secondary_unit` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | İkincil ölçü birimi desteği |
| `website_sale_product_item_cart_custom_qty` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Listeden özel adet ile sepete ekle |

### 💳 Ödeme & Checkout

| Modül | Repo | Ne Sağlar |
|---|---|---|
| `website_sale_acquirer_confirm_order` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Ödeme sağlayıcısına göre sipariş onayı |
| `website_sale_charge_payment_fee` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Ödeme işlem ücretini müşteriye yansıt |
| `website_sale_checkout_skip_payment` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Giriş yapmış kullanıcıya ödeme adımını atla |
| `website_sale_checkout_country_vat` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | KDV otomatik doldurma |
| `website_sale_require_legal` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Satın alımda yasal onay zorunluluğu |
| `website_sale_b2x_alt_price` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | KDV'li / KDV'siz alternatif fiyat |
| `website_sale_vat_required` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Checkout formunda KDV no zorunlu |
| `website_sale_tax_toggle` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Vergi görünümünü kullanıcı aç/kapat |

### 🎨 UX & Arayüz

| Modül | Repo | Ne Sağlar |
|---|---|---|
| `website_sale_category_breadcrumb` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Kategori kırıntı yolu (breadcrumb) |
| `website_sale_wishlist_keep` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Sepete ekle ama istek listesinde tut |
| `website_sale_wishlist_hide_price` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | İstek listesinde fiyat gizleme |
| `website_sale_suggest_create_account` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Misafire hesap oluşturma önerisi |
| `website_sale_comparison_hide_price` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Karşılaştırma sayfasında fiyat gizle |
| `website_sale_attribute_filter_form_submit` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Filtreleri manuel uygula |
| `website_sale_product_attribute_filter_category` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Özellik filtrelerini kategoriye göre grupla |
| `website_sale_order_shipping_modification` | [OCA/e-commerce](https://github.com/OCA/e-commerce) | Portaldan teslimat adresi değiştirme |

### 🔧 Backend & ERP (Ek OCA Repoları)

| Modül | Repo | Ne Sağlar |
|---|---|---|
| `sale_order_type` | [OCA/sale-workflow](https://github.com/OCA/sale-workflow) | Sipariş tipi yönetimi |
| `sale_discount_display_amount` | [OCA/sale-workflow](https://github.com/OCA/sale-workflow) | İndirim tutarını göster |
| `product_pricelist_direct_print` | [OCA/product-attribute](https://github.com/OCA/product-attribute) | Fiyat listesi yazdırma |
| `stock_available_to_promise_release` | [OCA/stock-logistics-workflow](https://github.com/OCA/stock-logistics-workflow) | Söz verilen stok yönetimi |
| `queue_job` | [OCA/queue](https://github.com/OCA/queue) | Asenkron iş kuyruğu |
| `connector_ecommerce` | [OCA/connector-ecommerce](https://github.com/OCA/connector-ecommerce) | ERP ↔ e-ticaret köprüsü |

---

## ❌ Adım 3 — Eksik Kalan Kısımlar (Bu Repodaki Custom Modüller)

OCA modülleri kurulduktan sonra aşağıdaki kritik alanlar **hâlâ eksik** kalır.  
Bu boşlukları doldurmak için bu repoda geliştirilen modüller:

### 💰 Ödeme Gateway'leri (Türkiye)

> OCA'da Türk ödeme sağlayıcısı entegrasyonu **bulunmamaktadır.**

| Modül (Bu Repo) | Açıklama |
|---|---|
| `payment_iyzico` | iyzico ödeme entegrasyonu — webhook, 3D Secure, iade |
| `payment_paytr` | PayTR sanal pos entegrasyonu |
| `payment_stripe_tr` | Stripe Türkiye uyumlu entegrasyon |

### 🚚 Kargo Entegrasyonları (Türkiye)

> OCA'da Türk kargo firması entegrasyonu **bulunmamaktadır.**

| Modül (Bu Repo) | Açıklama |
|---|---|
| `delivery_yurtici` | Yurtiçi Kargo — barkod, takip, etiket |
| `delivery_aras` | Aras Kargo entegrasyonu |
| `delivery_mng` | MNG Kargo entegrasyonu |
| `delivery_ptt` | PTT Kargo entegrasyonu |

### 🧾 SaaS & Abonelik Sistemi

> OCA'da tam SaaS abonelik / plan yönetimi **bulunmamaktadır.**

| Modül (Bu Repo) | Açıklama |
|---|---|
| `saas_subscription` | Plan yönetimi (free / pro / enterprise) |
| `saas_quota` | Kullanım kotası ve limit takibi |
| `saas_api_key` | API anahtar yönetimi |
| `saas_billing` | Periyodik fatura otomasyonu |

### 🔗 Headless API Katmanı

> Next.js / React frontend bağlantısı için REST API katmanı **bulunmamaktadır.**

| Modül (Bu Repo) | Açıklama |
|---|---|
| `website_sale_rest_api` | E-ticaret için REST API endpoint'leri |
| `website_sale_jwt_auth` | JWT tabanlı kimlik doğrulama |

---

## 🏗️ Önerilen Mimari

```
┌─────────────────────────────────────────────────────┐
│              Next.js / React Frontend               │
│         (Sipariş, sepet, kullanıcı paneli)          │
└──────────────────────┬──────────────────────────────┘
                       │ REST API / JSON-RPC
┌──────────────────────▼──────────────────────────────┐
│           Odoo Community 18.0 + OCA                 │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐ │
│  │  e-commerce │  │sale-workflow│  │    stock     │ │
│  │  (OCA free) │  │  (OCA free) │  │  (OCA free)  │ │
│  └─────────────┘  └─────────────┘  └─────────────┘ │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐ │
│  │payment_iyzico│ │delivery_     │  │saas_         │ │
│  │(bu repo)    │  │yurtici      │  │subscription  │ │
│  │             │  │(bu repo)    │  │(bu repo)     │ │
│  └─────────────┘  └─────────────┘  └─────────────┘ │
└─────────────────────────────────────────────────────┘
```

---

## 🚀 Hızlı Başlangıç

```bash
# 1. OCA e-commerce modüllerini klonla
git clone https://github.com/OCA/e-commerce.git --branch 18.0 addons/e-commerce

# 2. Bu repodaki custom modülleri ekle
git clone https://github.com/SENIN_KULLANICI/odoo-tr-ecommerce.git addons/tr-ecommerce

# 3. odoo.conf'a ekle
addons_path = addons/e-commerce,addons/tr-ecommerce

# 4. Modülleri yükle
./odoo-bin -d mydb -i website_sale_product_assortment,website_sale_stock_available,payment_iyzico
```

---

## 📊 Karşılanan İhtiyaçlar

| Alan | OCA Free | Bu Repo | Toplam |
|---|---|---|---|
| Ürün & Katalog | ✅ %100 | — | ✅ Tam |
| Stok Yönetimi | ✅ %80 | — | 🔶 İyi |
| UX / Arayüz | ✅ %70 | — | 🔶 İyi |
| Ödeme (Global) | 🔶 Kısmi | ✅ Bu repo | ✅ Tam |
| Ödeme (Türkiye) | ❌ Yok | ✅ Bu repo | ✅ Tam |
| Kargo (Türkiye) | ❌ Yok | ✅ Bu repo | ✅ Tam |
| SaaS Abonelik | ❌ Yok | ✅ Bu repo | ✅ Tam |
| Headless API | ❌ Yok | ✅ Bu repo | ✅ Tam |

---

## 🤝 Katkı

Bu proje OCA ruhunda geliştirilmektedir — tüm modüller **AGPL-3.0** lisansı ile ücretsiz dağıtılmaktadır.

Pull request ve issue'larınızı bekliyoruz.

---

## 📄 Lisans

AGPL-3.0 — Ticari projelerde ücretsiz kullanılabilir.
