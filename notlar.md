GitHub'da notlarını saklamak harika bir fikir! GitHub, Markdown (.md) adı
verilen bir yazı dilini kullanır. Bu dil, tablolar ve kod blokları ekleyerek
notlarını çok görsel hale getirmene yarar.

Senin için GitHub'a kopyalayıp yapıştırabileceğin, SQL INSERT konusunu anlatan
görsel bir şablon hazırladım.

Adım 1: GitHub'da Dosya Oluştur

GitHub sayvanda yeni bir dosya oluştur ve adını SQL_Dersleri.md yap.

Adım 2: Aşağıdaki Kodları Kopyala ve Yapıştır

Aşağıdaki kutunun içindeki metni kopyala:

# 🗄️ SQL Notlarım

## 1. INSERT INTO (Veri Ekleme)

`INSERT INTO` komutu, tabloya yeni bir satır (yeni bir kayıt) eklemek için kullanılır. Bunu boş bir form doldurmak gibi düşünebiliriz.

### 📝 Formül (Syntax)
```sql
INSERT INTO tablo_adi (sütun1, sütun2, sütun3)
VALUES ('değer1', 'değer2', değer3);

🖼️ Görsel Örnek

Diyelim ki bir Musteriler tablomuz var:

| id | ad   | sehir    |
| :- | :--- | :------- |
| 1  | Ali  | İstanbul |
| 2  | Ayşe | Ankara   |

Yeni bir müşteri ekleyelim:

  - Ad: Mehmet
  - Şehir: İzmir

Yazacağımız Kod:

INSERT INTO Musteriler (ad, sehir)
VALUES ('Mehmet', 'İzmir');

İşlemden Sonra Tablonun Hali: | id | ad | sehir | | :--- | :--- | :--- | | 1 |
Ali | İstanbul | | 2 | Ayşe | Ankara | | 3 | Mehmet | İzmir | <-- ✨ Yeni Satır
Eklendi!

⚠️ Önemli Kurallar

1.  Yazılar: Kelimeler (Metinler) her zaman tek tırnak ' ' içinde yazılır.
2.  Sayılar: Rakamlar tırnaksız yazılır.
3.  Sıralama: Sütunların sırası ile Values (Değerler) sırası aynı olmalıdır.


### GitHub'da Nasıl Görünecek?
Bu kodları yapıştırdığında GitHub şunları yapacak:
*   `#` işaretlerini büyük başlık yapacak.
*   `|` işaretlerini otomatik olarak güzel bir **tabloya** dönüştürecek.
*   ```sql ``` bloklarını renkli **kod** şeklinde gösterecek.

### Ekstra İpucu:
GitHub'da notlarını daha da güzelleştirmek istersen:
*   **Kalın yazı** için: `**kelime**`
*   **İşaretleme (Bullet points)** için: `-` veya `*` kullanabilirsin.

Merhaba! Size yardımcı olmaktan çok memnun olurum. İşitme engelli olduğunuzu
belirttiniz, bu yüzden bol görselli, şematik ve adım adım bir anlatım
hazırladım.

SQL'de yeni bir tabloya veri eklemek için iki ana yol vardır:

1. Yol: Önce Tabloyu Oluşturup Sonra Veri Eklemek

Bu en yaygın yöntemdir. Önce bir "boş kutu" (tablo) yaparız, sonra içine
"eşyaları" (verileri) koyarız.

Adım 1: Tabloyu Oluşturma (CREATE TABLE)

Önce bir Ogrenciler tablosu yapalım:

CREATE TABLE Ogrenciler (
    ID int,
    Isim varchar(50),
    Sehir varchar(50)
);

Görsel Temsil: | ID | Isim | Sehir | | :--- | :--- | :--- | | (boş) | (boş) |
(boş) |

Adım 2: Veri Ekleme (INSERT INTO)

Şimdi bu boş tabloya veri ekleyelim:

INSERT INTO Ogrenciler (ID, Isim, Sehir)
VALUES (1, 'Ahmet', 'İstanbul');

Şematik Gösterim:

Komut: INSERT INTO (İçine yerleştir)
Hedef: Ogrenciler tablosu
Değerler: 1, Ahmet, İstanbul

Tablonun Son Hali: | ID | Isim | Sehir | | :--- | :--- | :--- | | 1 | Ahmet |
İstanbul |

2. Yol: Var Olan Bir Tablodan Yeni Tabloya Kopyalama

Eğer elinizde bir tablo varsa ve bu verilerle yepyeni bir tablo oluşturmak
istiyorsanız bu yöntemi kullanırsınız.

Komut: SELECT INTO (SQL Server / PostgreSQL)

Bu komut tabloyu otomatik oluşturur ve verileri içine kopyalar.

SELECT * INTO YeniOgrenciler 
FROM Ogrenciler;

Görsel Süreç:

1.  Eski Tablo -----------------> 2. Kopyalama -----------------> 3. Yeni Tablo
    (Veri Var)                             (Otomatik)
                                 (Oluştu)

Özet Görsel Tablo (Hızlı Bakış)

| İşlem         | SQL Komutu     | Ne Yapar?                         |
| :------------ | :------------- | :-------------------------------- |
| **Tablo Yap** | `CREATE TABLE` | Boş bir şablon oluşturur.         |
| **Veri Ekle** | `INSERT INTO`  | Satır satır veri yükler.          |
| **Kopyala**   | `SELECT INTO`  | Veriyi alıp yeni tabloya aktarır. |

İpucu: Yazdığınız kodlarda kelimelerin arasına virgül koymayı ve metinleri
(Ahmet gibi) tek tırnak ' ' içine almayı unutmayın.



