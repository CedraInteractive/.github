# Güvenlik

## Açık bildirimi

Güvenlik açıklarını **issue olarak açmayın** — issue'lar depoya erişimi olan
herkese görünür ve açık düzeltilmeden yayılır.

Bunun yerine GitHub'ın özel bildirim kanalını kullanın:
ilgili deponun **Security → Report a vulnerability** sekmesi.

Kapalı kanal yoksa: **security@cedrainteractive.com**

Bildiriminizde şunlar olsun:

- Etkilenen depo ve sürüm (ya da commit SHA'sı)
- Tekrar üretme adımları
- Etkisi — bir saldırgan bununla ne yapabilir?

## Ne bekleyebilirsiniz

| Aşama | Süre |
|-------|------|
| İlk yanıt | 3 iş günü |
| Doğrulama ve etki değerlendirmesi | 7 gün |
| Düzeltme veya azaltma planı | ciddiyete göre |

Düzeltme yayınlanmadan açığı kamuya duyurmamanızı rica ederiz. Katkınız,
aksini istemediğiniz sürece sürüm notlarında anılır.

## Kapsam

Bu politika Cedra Interactive'in yayınladığı uygulamaları, oyunları ve
servisleri kapsar.

Kapsam dışı: üçüncü taraf servislerdeki açıklar (bunları o servise bildirin),
sosyal mühendislik, fiziksel erişim gerektiren senaryolar, ve kullanıcının
kendi cihazında root/jailbreak sonrası elde ettiği erişim.

## Anahtar sızıntısı

Bir imzalama anahtarı, keystore veya servis hesabı deposuna sızmışsa sıra
şudur: **önce anahtarı iptal edip yenisini üretin**, sonra geçmişi temizleyin.
Ters sırada temizlik yaparsanız anahtar zaten kopyalanmış olur.
