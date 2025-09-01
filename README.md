
# Orbis Status Page

> Self-hosted, single–file service-monitor dashboard that runs anywhere.

A zero-dependency (except a browser) status page that **pings your services every 5 s** and displays their latency + 60-minute uptime history in a dark, modern UI.

---

## ✨ Features

- **Real-time checks** via `HEAD` requests  
- **60-dot uptime history** for each service  
- **Dark glassmorphism UI** with Inter font  
- **Responsive** down to 320 px  
- **Keyboard shortcuts**  
  - `Space` – force refresh  
  - `?` – toggle help modal  
- **Zero build step** – drop in `index.html` and open it  
- **Under 15 kB** – one file, no trackers, no ads  

---

## ⚙️ Configuration

All settings live inside the HTML file; no external config.

| Option   | Default | Description |
|----------|---------|-------------|
| `services` | — | Array of `{name, url}` objects to monitor |
| `setInterval` delay | 5000 ms | How often to re-check all services |
| `ping` timeout | 10 000 ms | How long to wait before marking a service offline |

---

## 🧪 Hacking / Dev

- **Styling** – everything is in one `<style>` block (CSS + custom props).  
- **History length** – change `60` in `new Array(60)` to any number of dots.  
- **Edge functions / SSR** – if you want to prerender, the markup is minimal and easy to template.

---



   
