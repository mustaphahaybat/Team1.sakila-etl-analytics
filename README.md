
---

## 🧭 Proje Aşamaları ve Teslimatlar

### Phase 1 — MySQL -Orhan-
**Görevler**
- MySQL Workbench ile `sakila-schema.sql` ve `sakila-data.sql` import et.
- ERD oluştur (PNG).
- 5+ SQL sorgu hazırla ve sonuç ekran görüntülerini al.
- `customer`, `rental`, `payment` tablolarını CSV olarak export et.

**Teslimatlar**
- `docs/erd.png`
- `mysql/queries.sql`
- `data/customer.csv`, `data/rental.csv`, `data/payment.csv`
- Ekran görüntüleri (`docs/screenshots/`)

---

### Phase 2 — Snowflake -Mustafa-
**Görevler**
- Snowflake hesap, warehouse ve schema oluştur.
- `stage` oluşturup CSV’leri PUT + COPY INTO ile yükle.
- Star Schema tasarla: `fact_rental` ve dim tablolar (`dim_customer`, `dim_date`, `dim_film`, `dim_store`, vs.).
- 3 analitik sorgu çalıştır (ör: aylık gelir, ülkelere göre toplam ödeme, en çok kiralanan film/trend).

**Teslimatlar**
- `snowflake/star_schema.png`
- `snowflake/ddl.sql` (DDL + COPY INTO)
- `snowflake/analytics.sql` (analitik sorgular ve sonuç ekran görüntüleri)

---

### Phase 3 — MongoDB -Cafer-
**Görevler**
- MongoDB Atlas cluster oluştur.
- CSV’leri import et veya Snowflake’ten dönüştürülmüş JSON export et.
- Doküman modelini tasarla (embedded vs referenced kararları).
- Index’leri tanımla.
- 3 agregasyon sorgusu hazırla (ör: ülkeye göre kiralama sayısı, toplam ödemeler, aylık trend).

**Teslimatlar**
- `mongodb/doc_model.json`
- `mongodb/aggregations.js` veya `.txt`
- Ekran görüntüleri (`docs/screenshots/`)

---

## 👥 Takım ve Görev Dağılımı
- **Mustafa (Takım Lideri)** — Repo ve Trello yönetimi, Snowflake kurulumu, Star Schema tasarımı, final rapor.  
- **Orhan** — MySQL kurulumu, Sakila import, ERD, SQL sorguları, CSV export.  
- **Cafer** — MongoDB Atlas kurulumu, CSV import, JSON doküman tasarımı, agregasyon sorguları.

Ortak sorumluluklar:
- Her aşama için ekran görüntüsü almak.
- Dosyaları belirtilen klasörlere koymak.
- Trello kartlarını güncellemek.

---

## 📂 Klasör Yapısı (repo içinde)
