# Token Saver

Dosyalarını Claude'a yüklemeden önce sade Markdown'a çeviren, tamamen tarayıcıda çalışan bir araç. Bir PDF, Word ya da PowerPoint dosyasını olduğu gibi yüklediğinde içeriğin yanında biçimlendirmesi için de token ödersin. Bu araç biçimi atıp bilgiyi bırakır, böylece Claude aynı içeriği daha az token ile okur.

**Canlı kullan:** https://bahadir-digital.github.io/token-saver/

## Ne işe yarar

Daha az token; daha düşük maliyet ve kullanım limitlerine daha geç takılma demek. Tasarruf içerikten değil, dosyanın içindeki gereksiz biçim katmanından gelir, bu yüzden anlam korunur.

## Desteklenen dosyalar

- PDF
- Word (.docx)
- PowerPoint (.pptx)
- Excel (.xlsx)
- Metin (.txt, .md, .csv)

## Kullanımı

1. Aracı tarayıcıda aç.
2. Dosyanı sürükleyip bırak.
3. Oluşan Markdown'ı kopyala.
4. Ham dosya yerine bu metni Claude'a yapıştır.

## Tipik tasarruf

Aynı istem ve aynı çıktı ile yalnızca girdi biçimi değiştirilerek yapılan denemelerden gelen tahmini değerlerdir:

| Dosya türü | Tahmini tasarruf |
| --- | --- |
| PDF (metin ve görsel) | ~%70 |
| Word (.docx) | ~%50 |
| PowerPoint (.pptx) | ~%50 |
| Excel (.xlsx) | ~%40 |

Oranlar dosyadan dosyaya değişir.

## Gizlilik

Çevirme tamamen senin tarayıcında çalışır. Dosya hiçbir sunucuya gönderilmez, cihazından çıkmaz. Bu yüzden kurum içi belgelerle de kullanılabilir.

## Claude Skill

Bu depo aynı zamanda bir Claude Skill paketi içerir (`token-saver.skill`). Skill kurulduğunda, Claude ağır bir belgeyle çalışırken önce onu sade Markdown'a indirir ve tahmini token tasarrufunu raporlar. Kurmak için `.skill` dosyasını indirip Claude'a ekleyebilirsin.

## Depo içeriği

```
token-saver/
├── index.html          # Tarayıcıda çalışan çevirici (canlı sayfa)
├── token-saver.skill   # Kurulabilir Claude Skill paketi
└── README.md
```

## İletişim

- Blog: https://bahadir.digital
- LinkedIn: https://linkedin.com/in/bahadireren
- Claude.ai Türkiye topluluğu: https://chat.whatsapp.com/I2763pKIpmS9xADAHLaGPE
