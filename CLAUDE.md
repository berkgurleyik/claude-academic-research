# Claude Academic Research — çalışma kuralları

Bu repo hem Claude Code'un bulut çalışma alanı hem de GitHub Pages ile yayınlanan bir veri kaynağıdır.

## Klasörler
- `sources/` — PDF'ler, ham kaynaklar (yayınlanır; telifli PDF koyma, repo herkese açıksa görünür)
- `notes/` — Markdown araştırma notları, kaynak başına bir dosya: `notes/<id>.md`
- `data/` — Diğer uygulamaların çekeceği yapılandırılmış veri (JSON)
- `data/index.json` — `data/` içindeki tüm dosyaların listesi. **Her yeni veri dosyasında güncelle.**
- `data/dersler.json` — Dersler ve araştırma konuları; her konunun kaynak listesi `data/<konu>.json`
- `.claude/agents/akademik-arastirmaci.md` — Araştırma işleri için agent; kaynak bulma ve doğrulama kuralları orada

Notlardaki **"Benim notlarım"** bölümü kullanıcıya aittir; silme veya değiştirme, sadece ekle.

## Kurallar
- Yanıtlar ve notlar Türkçe; kaynak künyeleri orijinal dilinde.
- Her kaynak kaydı şu alanları içerir (`id`, `title`, `authors`, `year`, `type`, `tags`, `summary`, `notes_path`).
- Atıflarda APA 7 kullan. Doğrulayamadığın künyeyi uydurma; `"verified": false` ekle.
- JSON dosyalarını geçerli tut (virgül hatası yayındaki veriyi bozar).
- Değişiklikten sonra commit at ve push et; site birkaç dakika içinde güncellenir.
