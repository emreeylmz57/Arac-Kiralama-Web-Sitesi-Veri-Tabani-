# 🚗 Araç Kiralama Sistemi – SQL Veritabanı Projesi

Bu proje, çok şubeli bir araç kiralama firmasına ait ilişkisel veritabanı tasarımını içermektedir. Oracle SQL kullanılarak tablo yapıları, ilişkiler, örnek veriler ve otomatik hesaplama yapan bir trigger oluşturulmuştur.

---

## 📌 Proje Amacı

- Araç kiralama şirketi için ilişkisel veritabanı modeli oluşturmak  
- Şube, araç, müşteri ve kiralama ilişkilerini yönetmek  
- Kiralama işlemlerinde toplam ücret ve depozitoyu otomatik hesaplamak  
- Gerçekçi örnek veri seti ile sistemi test edebilmek  

---

## 🗂 Veritabanı Yapısı

Projede aşağıdaki tablolar bulunmaktadır:

- COMPANY  
- BRANCH  
- CATEGORY  
- CAR  
- CUSTOMER  
- ADDRESSES  
- RENT  

---

## 🔗 Temel İlişkiler

- Bir şirketin birden fazla şubesi vardır.  
- Bir şubede birden fazla araç bulunur.  
- Her araç bir kategoriye aittir.  
- Bir müşteri bir adrese bağlıdır.  
- Her kiralama işlemi bir müşteri ve bir araç ile ilişkilidir.  

---

## ⚙️ Trigger Mekanizması

`trg_depositAndTotalPriceCalculation` adlı trigger, RENT tablosuna yeni kayıt eklenmeden önce:

- Kiralama süresini otomatik hesaplar  
- Günlük araç ücretine göre toplam fiyatı belirler  
- Toplam fiyatın %10’u kadar depozitoyu otomatik hesaplar  

Bu sayede manuel hesaplama hataları önlenir ve veri bütünlüğü sağlanır.

---

## 🧪 Örnek Veri İçeriği

Projede:

- 1 şirket  
- 5 şube  
- 100+ araç  
- 80 müşteri  
- Çok sayıda kiralama kaydı  

Veriler test amaçlı oluşturulmuş olup gerçek hayata benzer senaryolar içermektedir.

---

## 🛠 Kullanılan Teknolojiler

- Oracle SQL  
- PL/SQL (Trigger)  
- İlişkisel Veritabanı Modelleme  

---

## 🚀 Kurulum ve Çalıştırma

1. SQL dosyasını Oracle SQL Developer ortamında açın.  
2. Script’i çalıştırın.  
3. Tablolar ve veriler otomatik olarak oluşturulacaktır.  
4. RENT tablosuna yeni kayıt ekleyerek trigger mekanizmasını test edebilirsiniz.  

---

## 📚 Bu Proje ile Öğrenilenler

- Relational database tasarımı  
- Primary & Foreign Key kullanımı  
- Trigger geliştirme  
- Veri bütünlüğü sağlama  
- Gerçekçi veri üretimi  
