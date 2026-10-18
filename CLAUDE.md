# Claude Academic Research — çalışma kuralları

Bu repo hem Claude Code'un bulut çalışma alanı hem de GitHub Pages ile yayınlanan bir veri kaynağıdır.

## Klasörler
- `sources/` — PDF'ler, ham kaynaklar (yayınlanır; telifli PDF koyma, repo herkese açıksa görünür)
- `notes/` — Markdown araştırma notları, kaynak başına bir dosya: `notes/<id>.md`
- `data/` — Diğer uygulamaların çekeceği yapılandırılmış veri (JSON)
- `data/index.json` — `data/` içindeki tüm dosyaların listesi. **Her yeni veri dosyasında güncelle.**

## Kurallar
- Yanıtlar ve notlar Türkçe; kaynak künyeleri orijinal dilinde.
- Her kaynak kaydı `data/example.json` şemasını izler (`id`, `title`, `authors`, `year`, `type`, `tags`, `summary`, `notes_path`).
- Atıflarda APA 7 kullan. Doğrulayamadığın künyeyi uydurma; `"verified": false` ekle.
- JSON dosyalarını geçerli tut (virgül hatası yayındaki veriyi bozar).
- Değişiklikten sonra commit at ve push et; site birkaç dakika içinde güncellenir.
