# CLAUDE.md — Odoo TR E-Ticaret (planlama reposu)

Odoo Community 17/18 + ücretsiz OCA modülleriyle e-ticaret kurulum rehberi ve **Türkiye'ye özgü eksik parçalar için planlanan custom modüller** (ödeme, kargo, SaaS abonelik, headless API). Repo şu an **sadece `README.md`** içeriyor — README'de "bu repodaki modüller" olarak listelenen modüllerin hiçbiri henüz yazılmadı.

- GitHub: https://github.com/SHapeloglu/e-commerce (tek yükleme, 2026-06-29)
- İlgili deneyim: `/opt/odoo` (Odoo 18 + `isg_addons`, `oca_social`), `l10n_tr_sovos_efatura`, `nakliye_yonetim_17v`, `n8nOdoo`.
- Mimari: `architect.md` · Görevler: `task.md` · Fikirler: `backlog.md` · Günlük: `session.md`

## Kurallar (modül yazımına başlanınca)

- Hedef sürüm **18.0** (README ve sunucudaki Odoo 18 ile uyumlu); her modül kendi klasöründe `__manifest__.py`, `models/`, `views/`, `security/ir.model.access.csv`, `data/`.
- Ödeme modülleri Odoo `payment` çerçevesini (`payment.provider`, `payment.transaction`) genişletir; kargo modülleri `delivery.carrier` (`<sağlayıcı>_rate_shipment`, `_send_shipping`, `_get_tracking_link`).
- API anahtarları / merchant bilgileri `payment.provider` / `delivery.carrier` alanlarında (kullanıcı arayüzünden girilir), koda veya data XML'ine yazılmaz.
- OCA kodlama kuralları (pre-commit, pylint-odoo) takip edilir; README'deki OCA modül listesi değişirse tabloyu güncelle.
- README'deki `git clone https://github.com/SENIN_KULLANICI/odoo-tr-ecommerce.git` yer tutucu — repo adı `SHapeloglu/e-commerce`.
- Oturum sonunda `session.md`'ye kayıt düş, `task.md`'yi güncelle.
