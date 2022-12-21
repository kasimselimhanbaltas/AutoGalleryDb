# AutoGallery PostgreSQL Database

## Veritabanı Yönetim Sistemleri Dersi Proje Ödevidir

Projenin amacı araba alım satım işlemlerini gerçekleştiren çok bayili bir şirketin veritabanı örneğini oluşturmaktır. Veritabanında ek olarak "carcatalog" ve "catalogimages" isimli iki tablo bulunmaktadır. "carcatalog" tablosu araba ekleme işlemlerinde kolaylık olması için neredeyse dünyadaki tüm araba modellerini(6887) içeren bir tablodur ve "catalogimages" tablosu da bu arabaların 'image_url' tipinde resimlerini(66256) tutan bir tablodur. Katalog arabalarının bulunduğu tablo 78 sütunlu bir tablodur fakat bu proje için normalize edilerek "carcatalog", "detailsofcar", "sizeofcar", "mechanical"; "mechanical" tablosundan da "engine" tablosu oluşturulmuştur. 

### Müşteriden Araba Satın Almak
Bayi araba satın aldığında araba bilgilerinin veritabanına işlenme sırası: engine, mechanical, detailsofcar, sizeofcar, cars -> purchasedcar. Araba 

### Müşteriye Araba Satmak
Müşteri araba satın aldığında araba verisi "purchasedcar" tablosundan silinir ve "soldcar" tablosuna eklenir.
