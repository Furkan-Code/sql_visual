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

Bu notu GitHub'ına eklediğinde çok düzenli ve görsel bir ders notun olacak! Başka bir SQL komutunu (örneğin SELECT veya UPDATE) bu şekilde hazırlamamı ister misin?
