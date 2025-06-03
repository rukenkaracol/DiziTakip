# DiziTakip

Aşko çok iyi gidiyosun, valla projen tam sunumluk olmuş! Sana GitHub linkli sade ve şık bir proje sunumu hazırlıyorum. Kopyala yapıştırla sunabilirsin ya da .pdf/.docx yaparsın istersen.

---

## 🎬 Dizi-Film Takip Sistemi

### 📌 Proje Linki:

[GitHub Repository](https://github.com/kullaniciAdin/projeAdi)
*(GitHub'daki kendi linkinle değiştir)*

---

### 📄 Proje Hakkında

Bu proje, kullanıcıların izledikleri dizi ve filmleri takip edebileceği bir masaüstü uygulamasıdır. Uygulama C# ve SQL Server kullanılarak geliştirilmiştir.

---

### 🛠️ Kullanılan Teknolojiler

* C# (.NET Windows Forms)
* SQL Server (Veritabanı)
* ADO.NET (SQL bağlantısı için)
* GitHub (Versiyon kontrol)

---

### 👤 Giriş / Kayıt Sistemi

* Kullanıcılar e-posta ve şifreyle giriş yapar.
* Üye olmayan kullanıcılar "Kayıt Ol" butonuyla sistemde hesap oluşturabilir.
* Adminler ayrı yetkilere sahiptir (içerik düzenleme vs.)

🖼️ *Ekran Görüntüsü:*
![frmGiris](attachment\:file-Kpphp6NVAjcs9gNDjPjRbB)

---

### 🎞️ Kullanıcı Paneli

* Tüm içerikler listelenir.
* İçerik arama, filtreleme ve puanlama yapılabilir.
* Kullanıcı yalnızca kendi izleme geçmişine erişebilir.
* İzleme durumu: "İzliyor", "Tamamlandı", "Bırakıldı" seçenekleriyle seçilebilir.

🖼️ *Ekran Görüntüsü:*
![frmKullanici](attachment\:file-DTFygs7CvbyxEUuiPQtcAH)

---

### 🛡️ Admin Paneli

* Yeni içerik ekleme
* İçerik güncelleme ve silme
* ContentID’ye göre tüm içerikler görüntülenebilir.

🖼️ *Ekran Görüntüsü:*
![frmAdmin](attachment\:file-UKiG2Qo5jQbmbTT9Sy45yx)

---

### 🧠 Veritabanı Tasarımı

* 3 Ana Tablo: `Users`, `Contents`, `WatchRecords`
* Kullanıcı, içerik ve izleme kayıtları arasında ilişkiler mevcuttur.

🖼️ *Veritabanı Şeması:*
![Veri Şeması](attachment\:file-KdyJyZXeNy98144MPf63co)

---

### 📌 İş Kuralları (Özet)

1. Kayıtsız kullanıcı sadece içerik görüntüleyebilir.
2. Kayıtlı kullanıcı içerik puanlayabilir, izleme durumunu değiştirebilir.
3. Bir içerik yalnızca bir kez puanlanabilir (güncellenebilir).
4. Kullanıcı sadece kendi geçmişini görebilir.
5. Silinen içerikler kullanıcı geçmişinde görünmez.

---

### 💾 Veritabanı Scripti

Projenin veritabanı yapısını oluşturan SQL dosyası GitHub reposunda yer almaktadır:
`SQLQuery21SON.sql`
*(ya da aşağıya örnek satır ekleyebilirsin)*

```sql
CREATE TABLE Users (
    UserID INT PRIMARY KEY IDENTITY(1,1),
    Email NVARCHAR(100) NOT NULL UNIQUE,
    Password NVARCHAR(100) NOT NULL,
    IsAdmin BIT NOT NULL
);
```

---

İstersen bu sunumu PowerPoint, Word ya da PDF'ye çevirebilirim. Renkli temalı versiyonunu da yaparız 💖
Hazır mısın? "Eline sağlık" diyip bırakmam, istersen sana *pptx veya pdf* olarak da export ederim. Hangisini istersin?
