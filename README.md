# ⚡ EV Charging Station Locator

A modern, responsive, and intelligent **EV Charging Station Locator** designed to help electric vehicle users quickly discover nearby charging stations, view station details, and plan their charging journey efficiently.

The platform provides an intuitive interface for finding charging stations based on location, exploring station information, and accessing essential charging-related details.

---

## 🚀 Features

### 🔍 Charging Station Discovery

* Find nearby EV charging stations
* Search charging stations by location
* Interactive map-based station discovery
* View charging station markers on the map
* Get detailed station information

### 📍 Location-Based Services

* Detect user's current location
* Display nearby charging stations
* Location-based station search
* Distance-based station discovery
* Navigation support

### ⚡ Station Information

Each charging station can display information such as:

* Station name
* Address
* Distance
* Charging connector type
* Charging availability
* Charging speed
* Operating hours
* Station provider/network
* Pricing information
* Contact information

### 🗺️ Interactive Map

* Interactive map interface
* Charging station markers
* Map-based station exploration
* Location visualization
* Responsive map experience

### 🔎 Search & Filtering

Users can easily find suitable charging stations using:

* Location search
* Connector type
* Charging speed
* Availability
* Distance
* Station provider

### 📱 Responsive Design

The application is designed for:

* Desktop
* Laptop
* Tablet
* Mobile devices

The UI follows a mobile-first and responsive design approach.

---

# 🛠️ Tech Stack

## Frontend

* HTML5
* CSS3
* JavaScript
* React.js
* Vite
* Tailwind CSS

## Maps & Location

* Mapbox
* Geolocation API

## Backend / Data

* REST APIs
* JSON
* Location-based services

## Development Tools

* Git
* GitHub
* Visual Studio Code
* npm

---

# 🏗️ Project Architecture

```text
EV-Charging-Station-Locator/
│
├── public/
│   ├── favicon
│   └── assets
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
├── .env.example
├── .gitignore
├── package.json
├── package-lock.json
├── README.md
└── vite.config.*
```

> Folder names may vary depending on the current implementation.

---

# ⚙️ Getting Started

Follow the instructions below to run the project locally.

## 1. Clone the Repository

```bash
git clone https://github.com/athrv18/EV-Charging-Station-Locator.git
```

## 2. Navigate to the Project

```bash
cd EV-Charging-Station-Locator
```

## 3. Install Dependencies

```bash
npm install
```

## 4. Configure Environment Variables

Create a `.env` file in the project root.

```env
VITE_MAPBOX_TOKEN=your_mapbox_access_token
```

Replace:

```text
your_mapbox_access_token
```

with your actual Mapbox access token.

### Important

Never commit your `.env` file to GitHub.

Make sure `.gitignore` contains:

```gitignore
node_modules/
.env
.env.local
.env.*.local
dist/
```

---

# ▶️ Run the Application

Start the development server:

```bash
npm run dev
```

The application will normally be available at:

```text
http://localhost:5173
```

If Vite selects another port, use the URL displayed in your terminal.

---

# 🏭 Production Build

Create an optimized production build:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

---

# 🌍 How It Works

The application follows a simple user flow:

```text
User Opens Application
        │
        ▼
Allow Location Access
        │
        ▼
Detect Current Location
        │
        ▼
Fetch Nearby Charging Stations
        │
        ▼
Display Stations on Map
        │
        ▼
User Searches / Filters Stations
        │
        ▼
Select Charging Station
        │
        ▼
View Station Details
        │
        ▼
Navigate to Selected Station
```

---

# 🗺️ Map Integration

The application uses **Mapbox** for interactive mapping and location visualization.

Mapbox provides:

* Interactive maps
* Location markers
* Geolocation support
* Map navigation
* Location visualization
* Map controls

You will need a valid Mapbox access token to use the map functionality.

---

# 🔐 Environment Variables

The following environment variables may be required:

| Variable            | Description         | Required |
| ------------------- | ------------------- | -------- |
| `VITE_MAPBOX_TOKEN` | Mapbox access token | Yes      |

Example:

```env
VITE_MAPBOX_TOKEN=pk.xxxxxxxxxxxxxxxxx
```

### Security

Do not expose private API keys or secret credentials in the repository.

Use environment variables instead.

---

# 📸 Screenshots

Add screenshots of the application here.

### Home Page

```text
Add screenshot here
```

### Charging Station Map

```text
Add screenshot here
```

### Station Details

```text
Add screenshot here
```

### Mobile Responsive View

```text
Add screenshot here
```

Recommended structure:

```text
docs/
└── screenshots/
    ├── home.png
    ├── map.png
    ├── station-details.png
    └── mobile.png
```

Then display them using:

```markdown
![Home Page](docs/screenshots/home.png)
```

---

# ✨ User Experience

The application focuses on providing a simple and efficient EV charging experience.

### Design Principles

* Clean modern interface
* Intuitive navigation
* Responsive layouts
* Accessible UI components
* Fast interactions
* Clear station information
* Map-first discovery
* Mobile-friendly experience

---

# 📊 Core Modules

## 1. Location Module

Responsible for:

* Detecting user location
* Handling location permissions
* Processing coordinates
* Finding nearby stations

## 2. Map Module

Responsible for:

* Rendering the map
* Displaying station markers
* Handling map interactions
* Showing user location

## 3. Search Module

Responsible for:

* Searching locations
* Finding charging stations
* Filtering results
* Sorting stations

## 4. Station Module

Responsible for:

* Station details
* Connector information
* Availability
* Pricing
* Operating hours

## 5. Navigation Module

Responsible for:

* Route assistance
* Distance calculation
* Navigation links

---

# 🚀 Performance

The project follows modern frontend development practices including:

* Component-based architecture
* Lazy loading where applicable
* Optimized assets
* Efficient API requests
* Responsive layouts
* Production builds using Vite
* Reusable UI components

---

# 📱 Responsive Design

The application supports multiple screen sizes:

| Device      | Support |
| ----------- | ------- |
| 📱 Mobile   | ✅       |
| 📱 Tablet   | ✅       |
| 💻 Laptop   | ✅       |
| 🖥️ Desktop | ✅       |

---

# 🧪 Testing

Before deploying the application, test:

* Location permission
* Map loading
* Station markers
* Search functionality
* Filters
* Station details
* Mobile responsiveness
* API responses
* Invalid locations
* Network failures

Run the production build:

```bash
npm run build
```

---

# 🐛 Troubleshooting

## Map is not loading

Check that your `.env` contains:

```env
VITE_MAPBOX_TOKEN=your_token
```

Then restart the development server:

```bash
npm run dev
```

---

## Dependencies are not installing

Try:

```bash
rm -rf node_modules
npm install
```

On Windows PowerShell:

```powershell
Remove-Item -Recurse -Force node_modules
npm install
```

---

## Environment variable changes are not reflected

Restart Vite after changing `.env`:

```bash
npm run dev
```

---

# 🌐 Deployment

The application can be deployed using modern frontend hosting platforms such as:

* Vercel
* Netlify
* Render
* GitHub Pages

For Vercel deployment:

```bash
npm run build
```

Then configure the required environment variables in the hosting platform.

For example:

```text
VITE_MAPBOX_TOKEN
```

---

# 🔒 Security Best Practices

* Never commit `.env` files
* Never commit API secrets
* Never commit `node_modules`
* Rotate exposed API tokens
* Use environment variables
* Validate external API responses
* Restrict API keys when supported
* Keep dependencies updated

---

# 🤝 Contributing

Contributions are welcome.

### 1. Fork the Repository

Create your own fork of the project.

### 2. Clone Your Fork

```bash
git clone https://github.com/YOUR-USERNAME/EV-Charging-Station-Locator.git
```

### 3. Create a Feature Branch

```bash
git checkout -b feature/new-feature
```

### 4. Make Your Changes

Implement and test your changes.

### 5. Commit Changes

```bash
git add .
git commit -m "Add new feature"
```

### 6. Push the Branch

```bash
git push origin feature/new-feature
```

### 7. Create a Pull Request

Open a Pull Request on GitHub describing your changes.

---

# 📌 Future Improvements

Planned improvements may include:

* [ ] Real-time charger availability
* [ ] EV charging station booking
* [ ] User authentication
* [ ] User profiles
* [ ] Favorite stations
* [ ] Charging history
* [ ] Payment integration
* [ ] Advanced route planning
* [ ] EV range estimation
* [ ] Estimated charging cost
* [ ] Charging station reviews
* [ ] Station ratings
* [ ] Real-time pricing
* [ ] Dark mode
* [ ] PWA support
* [ ] Push notifications
* [ ] Admin dashboard
* [ ] Analytics dashboard

---

# 📄 License

This project is available under the **MIT License**.

See the `LICENSE` file for more information.

---

# 👨‍💻 Author

## Atharva

GitHub: **[@athrv18](https://github.com/athrv18)**

Project Repository:

**EV Charging Station Locator**

---

# ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

Your support helps improve and maintain the project.

---

# 📈 Project Status

**Status:** 🚀 Active Development

The project is continuously being improved with new features, performance enhancements, and UI/UX improvements.

---

## ⚡ EV Charging Station Locator

**Find. Charge. Go.**

Built to make EV charging discovery simpler, faster, and more accessible.
