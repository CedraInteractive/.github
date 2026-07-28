# Katkı

Bu kurallar Cedra Interactive'in bütün depoları için geçerlidir. Bir depoda
kendi `CONTRIBUTING.md`'si varsa o öncelikli.

## Commit

[Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): description
```

| Tip | Ne zaman |
|-----|----------|
| `feat` | yeni davranış |
| `fix` | bozuk olanı düzeltme |
| `refactor` | davranış değişmiyor, yapı değişiyor |
| `perf` | ölçülmüş hızlanma |
| `build` | derleme sistemi, bağımlılık |
| `ci` | workflow, hook |
| `docs` | belge |
| `test` | test |
| `chore` | bakım, temizlik |

Başlık 72 karakteri geçmesin ve **ne yaptığını değil neyi çözdüğünü** söylesin.
Gövde varsa gerekçeyi taşısın: kod ne yaptığını zaten anlatıyor, neden
yapıldığını anlatmıyor.

`Co-Authored-By` satırı eklenmez.

## Dal

- `main` — kararlı
- `feat/<konu>`, `fix/<konu>` — özellik dalları

Bir depoda birden fazla ürün tutulmaz. Ürün başına depo; ortak kod şablon
deposundan dosya bazında taşınır.

## Pull request

Şablon otomatik gelir. Üç şeyi doldurun: ne değişti, neden, nasıl doğrulandı.
Üçüncüsü "test edildi" değil — hangi cihazda hangi turu attığınız.

Derleme geçmeden merge edilmez.

## Asla commit edilmeyecekler

- `.env`, `*.key`, `*.pem`, `*.pfx`, `*.keystore`, `keystore.properties`
- API anahtarı, servis hesabı JSON'ı, imzalama materyali
- Üretilen dosyalar: `build/`, `.cxx/`, `node_modules/`, `*.apk`, `*.aab`, `*.exe`
- 5 MB üzeri ikili dosyalar — CDN'e koyun

Bir secret yanlışlıkla girerse: **anahtarı iptal edin**, sonra geçmişten
temizleyin. Sıra bu; ters sırada anahtar zaten sızmış olur.

## Kayıt dosyasına yazılan değerler

Kayıt dosyasına yazılan enum'lar yeniden numaralandırılmaz. Değeri kayan bir
enum, oyuncunun kaydını sessizce bozar — yeni değer sona eklenir.
