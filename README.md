# 🌍 World Wildlife Population Monitoring System (WWPMS)

An interactive geospatial web platform for real-time wildlife species monitoring, extinction risk assessment, and biodiversity conservation awareness.

---

## 🚀 Live Demo
> Deploy to GitHub Pages — see setup below.

---

## 📸 Features

- 🗺️ **Interactive World Map** — Satellite, Esri Imagery, Topographic, and Forest Cover layers
- 📍 **Color-coded Species Markers** — Instantly identify threat level at a glance
- 🔥 **Endangered Species Heatmap** — Visualise endangered zones globally
- 🔍 **Smart Search** — Search by species name, continent, type, or threat status
- 🎛️ **Filter Panel** — Filter by continent or endangerment level
- 📊 **Live Stats Bar** — Real-time count of species by threat status
- 📦 **Data-driven Architecture** — All species data loaded from `animals.json` (no hardcoded JS)
- 📱 **Responsive Design** — Works on desktop, tablet, and mobile

---

## 🐾 Species Covered (26+)

| Continent | Species |
|-----------|---------|
| Asia | Bengal Tiger, Indian Elephant, Snow Leopard, Asiatic Lion, Gharial, Indian Pangolin, Indian Peacock, Indian Cobra, Indian Star Tortoise |
| Africa | African Elephant, Lion, Cheetah, Rhinoceros, Giraffe |
| Oceania | Kangaroo, Koala, Tasmanian Devil, Kakapo, Kiwi |
| South America | Jaguar, Andean Condor, Magellanic Penguin, Maned Wolf |
| North America | White-tailed Deer, Moose, Reindeer |

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| HTML5, CSS3, Vanilla JavaScript | Core frontend |
| [Leaflet.js](https://leafletjs.com/) | Interactive maps |
| [Leaflet.heat](https://github.com/Leaflet/Leaflet.heat) | Heatmap overlay |
| [Leaflet Control Geocoder](https://github.com/perliedman/leaflet-control-geocoder) | Location search |
| [MapTiler](https://www.maptiler.com/) | Hybrid satellite tiles |
| [Esri World Imagery](https://www.esri.com/) | Alternative satellite layer |
| `animals.json` | External species data (no hardcoded JS) |
| Wikimedia Commons | Hosted species images |

---

## 📁 Project Structure

```
wwpms/
├── index.html       # Main application
├── animals.json     # All species data (external, scalable)
└── README.md        # This file
```

---

## ⚙️ Setup & Run Locally

```bash
# Clone the repo
git clone https://github.com/Lavanyachawda/World-wildlife-population-monitoring-system.git
cd World-wildlife-population-monitoring-system

# Serve locally (required for fetch() to load animals.json)
# Option 1: Python
python -m http.server 8000

# Option 2: Node.js
npx serve .

# Then open: http://localhost:8000
```

> ⚠️ You must use a local server — opening `index.html` directly in a browser will block `fetch()` due to CORS.

---

## 🌐 Deploy to GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Set source to `main` branch, `/ (root)` folder
3. Click **Save** — your site will be live at:
   `https://lavanyachawda.github.io/World-wildlife-population-monitoring-system/`

---

## 🔮 Future Improvements

- [ ] Connect to [IUCN Red List API](https://apiv3.iucnredlist.org/) for live population data
- [ ] Add population trend charts per species (Chart.js)
- [ ] User sighting reports (crowdsourced data)
- [ ] Species comparison tool

---

## 👩‍💻 Author

**Lavanya Chawda** — [GitHub](https://github.com/Lavanyachawda) | [LinkedIn](#)

---

## 📄 License

MIT License — feel free to use and build upon this project.
