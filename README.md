# # Atikaku PHP + FPDF Projesi

## Klasör Yapısı

```
/ (proje kökü)
|-- public/           # Dışarıya açık dosyalar (index.php, resimler)
|-- src/              # Kendi PHP kodlarınız (iş mantığı, controller vs.)
|-- fpdf/             # FPDF kütüphanesi (dışarıya kapalı)
|-- output/           # Oluşturulan PDF dosyaları
|-- image/            # Resimler (kullanıma göre public'e taşınabilir)
|-- .well-known/      # SSL ve diğer sistem klasörleri
|-- cgi-bin/          # (Varsa özel CGI scriptleri)
```

## Kurulum

1. PHP 7.4+ kurulu olmalı.
2. FPDF kütüphanesi `fpdf/` klasöründe hazır.
3. `public/` klasöründeki `index.php` ile örnek PDF oluşturabilirsiniz.

## Kullanım

- Tarayıcıda `public/index.php` dosyasını açarak test edebilirsiniz.
- Oluşturulan PDF dosyaları `output/` klasörüne kaydedilir.

## Güvenlik

- `fpdf/`, `src/` ve `output/` klasörlerine doğrudan erişim engellenmelidir (htaccess veya sunucu ayarları ile).

## Geliştirme

- Kendi iş mantığınızı `src/` klasöründe geliştirin.
- Yeni özellikler için kodunuzu modüler tutun.
