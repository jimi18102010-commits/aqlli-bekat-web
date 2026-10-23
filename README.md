# Aqlli Bekat Web

Scrollsiz Toshkent bekat interfeysi. Vanilla HTML/CSS/JS, Leaflet, OpenStreetMap.

## Ishga tushirish (Windows)

`index.html` ni Edge yoki Chrome’da oching. Tavsiya etilgan ekran: 1366×768 yoki kattaroq; mobil interfeys alohida ko‘rinishlarga bo‘lingan. Internet xarita, manzil qidirish va yo‘l hisoblash uchun kerak. Buyruq satri shart emas.

HTTP server orqali: `python -m http.server 8080` va `http://localhost:8080`.

## Imkoniyatlar

- 100dvh scrollsiz desktop/mobil layout; mobil tablar.
- Haqiqiy OSM xaritasi, Leaflet.
- Transport simulyatsiyasi (aniq sinov belgisi bilan), avtobus tanlash va kuzatish.
- Photon yordamida Toshkent hududida manzil qidirish (submit, autocomplete yo‘q).
- Xaritadan nuqta tanlash va OSRM orqali avtomobil yo‘li.
- Jamoat transporti uchun Yandex Maps tashqi havolasi.
- Reklama aylanishi, ixtiyoriy ovoz, localStorage sozlamalari.
- Ketishlar jurnali, pagination, loading/error/empty holatlari.

## Muhim cheklovlar

Bu production transport backend’i emas. Raqamlar, bekat, marshrut chiziqlari, kelish va ketishlar sun’iy. Hech qanday yashirin Yandex API ishlatilmaydi. Jonli GPS va rasmiy yo‘nalishlar uchun huquqiy ruxsat va operator integratsiyasi kerak. OSRM yo‘li avtomobil uchun, avtobus yo‘li emas. Trafik hisobga olinmaydi. Tezkor manzillar nuqtalari taxminiy kirish joylari.

Photon, OSRM va OSM ommaviy xizmatlari SLA bermaydi; ishlab chiqarish uchun shartnomali yoki o‘z serveringizdagi xizmat, monitoring va foydalanish siyosatlariga muvofiqlik zarur. Qidiruv so‘rovi Photon’ga, koordinatalar OSRM’ga yuboriladi. Xarita yuklanishi IP va tile so‘rovlarini OSM’ga yuboradi. Qidiruv natijalari sessiya keshida. Reklama hisob-kitobi va loginli admin hali yo‘q.

## Hosting

GitHub Actions workflow GitHub Pages’ga joylash uchun kiritilgan. Repository Settings → Pages → Source: GitHub Actions. So‘ng Actions → Deploy website → Run workflow. Pages o‘chirilgan bo‘lsa bir marta Settings’da yoqish talab etilishi mumkin.

## Attribution

© OpenStreetMap contributors (https://www.openstreetmap.org/copyright). Leaflet © Vladimir Agafonkin va hamkorlar — BSD-2-Clause. Photon © komoot / OSM; yo‘l hisoblash OSRM. Kiosk ko‘paytirilishidan oldin provayderlar siyosati va kvotalarini tekshiring.
