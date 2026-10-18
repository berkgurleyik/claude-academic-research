# Claude Academic Research

Akademik araştırma çalışma alanı. Claude Code (claude.ai/code) ile her cihazdan düzenlenir, GitHub Pages ile yayınlanır.

## Veriye dışarıdan erişim
Pages açıldıktan sonra adresler:

- Ana sayfa: `https://<kullanıcı-adın>.github.io/claude-academic-research/`
- Dosya listesi: `https://<kullanıcı-adın>.github.io/claude-academic-research/data/index.json`
- Tek dosya: `https://<kullanıcı-adın>.github.io/claude-academic-research/data/<dosya>.json`

Her uygulama (Python, Excel/Power Query, Google Sheets `IMPORTDATA`, Zapier, n8n vb.) bu adreslerden düz HTTP GET ile veri çekebilir.

Örnek (Python):
```python
import requests
idx = requests.get("https://<kullanıcı-adın>.github.io/claude-academic-research/data/index.json").json()
for f in idx["files"]:
    print(f["title"], f["path"])
```
