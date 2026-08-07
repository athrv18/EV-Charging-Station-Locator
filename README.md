# ⚡ EV Charging Station Locator

<p align="center">
  <strong>Find. Charge. Go.</strong>
</p>

<p align="center">
  A modern, responsive, and location-based EV Charging Station Locator that helps electric vehicle users discover nearby charging stations quickly and efficiently.
</p>

<p align="center">
  <a href="https://github.com/athrv18/EV-Charging-Station-Locator">
    <img src="https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github" alt="GitHub">
  </a>
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React">
  <img src="https://img.shields.io/badge/Vite-7-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-3-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/Mapbox-Maps-000000?style=for-the-badge&logo=mapbox&logoColor=white" alt="Mapbox">
</p>

---

## 📖 Overview

**EV Charging Station Locator** is a web application designed to simplify the process of finding electric vehicle charging stations.

The platform combines **interactive maps, location services, search, filtering, and charging station information** into a single user-friendly interface.

Users can discover nearby charging stations, explore station details, and identify suitable charging locations based on their requirements.

---

## ✨ Key Features

### 🔍 Charging Station Discovery

* Find nearby EV charging stations
* Search stations by location
* Interactive map-based discovery
* Display charging station markers
* View detailed station information

### 📍 Location-Based Services

* Detect user's current location
* Display nearby charging stations
* Location-based station search
* Distance-based station discovery
* Navigation support

### ⚡ Charging Station Information

Depending on the available station data, users can view:

* Station name
* Address
* Distance
* Charging connector type
* Charging speed
* Charging availability
* Operating hours
* Station provider/network
* Pricing information
* Contact information

### 🗺️ Interactive Map

* Interactive Mapbox map
* Charging station markers
* User location visualization
* Map navigation controls
* Location-based exploration
* Responsive map interface

### 🔎 Search & Filtering

Users can find relevant charging stations using:

* Location
* Distance
* Connector type
* Charging speed
* Availability
* Station provider

### 📱 Fully Responsive

Designed to work across:

* 📱 Mobile
* 📲 Tablet
* 💻 Laptop
* 🖥️ Desktop

The interface follows a responsive and mobile-first design approach.

---

# 🛠️ Tech Stack

| Technology          | Purpose                     |
| ------------------- | --------------------------- |
| **React.js**        | Frontend UI                 |
| **Vite**            | Development & build tooling |
| **Tailwind CSS**    | Styling & responsive design |
| **JavaScript**      | Application logic           |
| **Mapbox**          | Interactive maps            |
| **Geolocation API** | User location               |
| **REST APIs**       | Station/location data       |
| **JSON**            | Data handling               |
| **npm**             | Package management          |
| **Git & GitHub**    | Version control             |
| **VS Code**         | Development environment     |

---

# 🏗️ Project Structure

```text
EV-Charging-Station-Locator/
│
├── public/
│   ├── favicon
│   └── assets/
│
├── src/
│   ├── components/
│   ├── pages/
│   ├── services/
│   ├── hooks/
│   ├── utils/
│   ├── assets/
│   ├── styles/
│   ├── App.*
│   └── main.*
│
├── docs/
│   └── screenshots/
│
├── .env.example
├── .gitignore
├── package.json
├── package-lock.json
├── README.md
└── vite.config.*
```

> The exact folder structure may vary depending on the current implementation.

---

# ⚙️ Getting Started

Follow the steps below to run the project locally.

## Prerequisites

Make sure you have installed:

* **Node.js 20+**
* **npm**
* **Git**
* A **Mapbox access token**

Check your versions:

```bash
node --version
npm --version
git --version
```

---

## 1. Clone the Repository

```bash
git clone https://github.com/athrv18/EV-Charging-Station-Locator.git
```

---

## 2. Navigate to the Project

```bash
cd EV-Charging-Station-Locator
```

---

## 3. Install Dependencies

```bash
npm install
```

---

## 4. Configure Environment Variables

Create a `.env` file in the project root:

```env
VITE_MAPBOX_TOKEN=your_mapbox_access_token
```

Replace `your_mapbox_access_token` with your actual Mapbox token.

### 🔐 Important

Never commit `.env` to GitHub.

Your `.gitignore` should include:

```gitignore
node_modules/
.env
.env.local
.env.*.local
dist/
build/
```

---

# ▶️ Run the Application

Start the development server:

```bash
npm run dev
```

Vite will display the local development URL in your terminal.

Example:

```text
http://localhost:5173
```

---

# 🏭 Production Build

Create an optimized production build:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

---

# 🌍 Application Workflow

```text
┌─────────────────────────┐
│      Open Application   │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│   Allow Location Access │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│  Detect Current Location│
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Find Nearby Stations    │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Display Stations on Map │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Search / Filter Results │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Select Charging Station │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ View Station Details    │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Navigate to Station     │
└─────────────────────────┘
```

---

# 🗺️ Map Integration

The application uses **Mapbox** for interactive mapping and location visualization.

Mapbox enables:

* Interactive maps
* Charging station markers
* Location visualization
* Map navigation
* User location display
* Map controls
* Location-based exploration

A valid Mapbox access token is required for map functionality.

---

# 🔐 Environment Variables

| Variable            | Description         | Required |
| ------------------- | ------------------- | :------: |
| `VITE_MAPBOX_TOKEN` | Mapbox access token |     ✅    |

Example:

```env
VITE_MAPBOX_TOKEN=pk.xxxxxxxxxxxxxxxxx
```

### Security Guidelines

Never commit:

* API keys
* Access tokens
* Passwords
* `.env` files
* Private credentials

Use environment variables for sensitive configuration.

---

# 📸 Screenshots

> Add your actual project screenshots inside `docs/screenshots/`.

### 🏠 Home Page

![Home Page](docs/screenshots/home.png)

### 🗺️ Charging Station Map

![Charging Station Map](docs/screenshots/map.png)

### ⚡ Station Details

![Station Details](docs/screenshots/station-details.png)

### 📱 Mobile View

![Mobile Responsive View](docs/screenshots/mobile.png)

---

# ✨ UI/UX Design

The application focuses on delivering a clean and efficient EV charging discovery experience.

### Design Principles

* Modern interface
* Responsive layouts
* Intuitive navigation
* Accessible UI
* Clear information hierarchy
* Fast interactions
* Map-first discovery
* Mobile-friendly experience
* Reusable components

---

# 📊 Core Modules

## 📍 Location Module

Responsible for:

* Detecting user location
* Handling location permissions
* Processing coordinates
* Finding nearby charging stations

## 🗺️ Map Module

Responsible for:

* Rendering the map
* Displaying charging stations
* Handling map interactions
* Showing user location

## 🔎 Search Module

Responsible for:

* Location search
* Station search
* Filtering
* Sorting
* Distance-based discovery

## ⚡ Station Module

Responsible for:

* Station details
* Connector information
* Charging speed
* Availability
* Pricing
* Operating hours

## 🧭 Navigation Module

Responsible for:

* Distance calculation
* Navigation links
* Route assistance

---

# 🚀 Performance

The project follows modern frontend development practices including:

* Component-based architecture
* Reusable components
* Optimized assets
* Efficient API requests
* Responsive layouts
* Vite production builds
* Environment-based configuration
* Maintainable project structure

---

# 📱 Responsive Support

| Device      | Support |
| ----------- | :-----: |
| 📱 Mobile   |    ✅    |
| 📲 Tablet   |    ✅    |
| 💻 Laptop   |    ✅    |
| 🖥️ Desktop |    ✅    |

---

# 🧪 Testing Checklist

Before deployment, verify:

* [ ] Application loads correctly
* [ ] Map loads successfully
* [ ] Location permission works
* [ ] User location is detected
* [ ] Charging station markers appear
* [ ] Search works correctly
* [ ] Filters work correctly
* [ ] Station details load
* [ ] Navigation works
* [ ] Mobile layout works
* [ ] Tablet layout works
* [ ] Desktop layout works
* [ ] API failures are handled
* [ ] Invalid locations are handled
* [ ] Production build succeeds

Run:

```bash
npm run build
```

---

# 🐛 Troubleshooting

## Map is not loading

Verify your `.env` file:

```env
VITE_MAPBOX_TOKEN=your_mapbox_access_token
```

Then restart the development server:

```bash
npm run dev
```

---

## Dependencies are not installing

### Windows PowerShell

```powershell
Remove-Item -Recurse -Force node_modules
Remove-Item package-lock.json
npm install
```

### macOS / Linux

```bash
rm -rf node_modules
rm package-lock.json
npm install
```

---

## Environment variable changes are not reflected

Restart the Vite development server:

```bash
npm run dev
```

---

# 🌐 Deployment

The project can be deployed using platforms such as:

* Vercel
* Netlify
* Render
* GitHub Pages

Before deployment:

```bash
npm run build
```

Configure your production environment variable:

```text
VITE_MAPBOX_TOKEN
```

Do not upload the `.env` file.

---

# 🔒 Security Best Practices

* ✅ Never commit `.env`
* ✅ Never commit API secrets
* ✅ Never commit `node_modules`
* ✅ Use environment variables
* ✅ Rotate exposed credentials
* ✅ Restrict API keys when possible
* ✅ Validate API responses
* ✅ Keep dependencies updated
* ✅ Use HTTPS in production

---

# 🤝 Contributing

Contributions are welcome.

## 1. Fork the Repository

Create a fork of the project on GitHub.

## 2. Clone Your Fork

```bash
git clone https://github.com/YOUR-USERNAME/EV-Charging-Station-Locator.git
```

## 3. Create a Feature Branch

```bash
git checkout -b feature/new-feature
```

## 4. Make Your Changes

Implement and test your changes.

## 5. Commit Your Changes

```bash
git add .
git commit -m "Add new feature"
```

## 6. Push Your Branch

```bash
git push origin feature/new-feature
```

## 7. Open a Pull Request

Create a Pull Request on GitHub with a clear description of your changes.

---

# 🗺️ Roadmap

Future improvements may include:

* [ ] Real-time charger availability
* [ ] EV charging station booking
* [ ] User authentication
* [ ] User profiles
* [ ] Favorite stations
* [ ] Charging history
* [ ] Payment integration
* [ ] Advanced route planning
* [ ] EV range estimation
* [ ] Charging cost estimation
* [ ] Station reviews
* [ ] Station ratings
* [ ] Real-time pricing
* [ ] Dark mode
* [ ] PWA support
* [ ] Push notifications
* [ ] Admin dashboard
* [ ] Analytics dashboard

---

# 📄 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for complete license information.

---

# 👨‍💻 Author

## Atharva

GitHub: [@athrv18](https://github.com/athrv18)

Repository: [EV Charging Station Locator](https://github.com/athrv18/EV-Charging-Station-Locator)

---

# ⭐ Support

If you find this project useful, please consider giving the repository a ⭐ on GitHub.

Your support is greatly appreciated!

---

# 📈 Project Status

**Status:** 🚀 Active Development

The project is continuously being improved with new features, performance optimizations, and UI/UX enhancements.

---

<div align="center">

### ⚡ EV Charging Station Locator

**Find. Charge. Go.**

Built to make EV charging discovery **simpler, faster, and more accessible.**

</div>
