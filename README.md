<p align="center">
  <img src="https://raw.githubusercontent.com/Omarsalama2001/islamina_demo/main/ic_launcher.png"
       width="200" 
       alt="Islamina Logo"/>
</p>

<h1 align="center">Islamina</h1>
<p align="center">
  A comprehensive Islamic Flutter app featuring Quran reading, prayer times, Khatma tracker, digital Tasbih, and live Quran radio streaming.
</p>

<p align="center">
  <a href="https://github.com/Omarsalama2001/islamina_app">
    <img src="https://img.shields.io/badge/GitHub-View%20Code-100000?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <img src="https://img.shields.io/badge/Flutter-Mobile-02569B?style=for-the-badge&logo=flutter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
</p>

---

## ✨ Features

<table>
  <tr>
    <td align="center" width="50%">
      <h3>🕌 Prayer Times</h3>
      <p>Accurate daily prayer times based on your current location with multiple calculation methods and Madhab support</p>
    </td>
    <td align="center" width="50%">
      <h3>📖 Holy Quran</h3>
      <p>Full Quran with a smooth and beautiful reading experience, supporting multiple fonts and display settings</p>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <h3>🎙️ Quran Audio Player</h3>
      <p>Listen to the Holy Quran with <strong>10+ world-renowned reciters</strong> with full playback controls</p>
    </td>
    <td align="center" width="50%">
      <h3>📚 Quran Tafsir</h3>
      <p>Quran Tafsir available in <strong>different languages</strong> for a deeper understanding of the Quran</p>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <h3>📿 Digital Tasbih</h3>
      <p>Animated digital Tasbih that feels like a real one, with customizable Azkar and counter settings</p>
    </td>
    <td align="center" width="50%">
      <h3>📔 Khatma Tracker</h3>
      <p>Track your Quran reading progress with <strong>cloud sync</strong> across all your devices using the same account</p>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <h3>🧭 Qibla Finder</h3>
      <p>Accurate Qibla direction with real-time compass and distance from the Holy Mosque in Makkah</p>
    </td>
    <td align="center" width="50%">
      <h3>📻 Quran Radio</h3>
      <p>Live streaming of the most famous Quran radio stations including <strong>Egypt, Saudi Arabia</strong> and more</p>
    </td>
  </tr>
</table>

---

## 🛠️ Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white"/>
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/GetX-8B0000?style=for-the-badge&logo=flutter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Flutter_Bloc-02569B?style=for-the-badge&logo=flutter&logoColor=white"/>
</p>

---

## 🏗️ Architecture

This app is built using **Clean Architecture** pattern:

| Layer | Responsibility |
|-------|---------------|
| 📊 **Data** | Remote & Local data sources, Models, Repository implementations |
| 🧠 **Domain** | Entities, Repository interfaces, Use cases (Business logic) |
| 🎨 **Presentation** | UI Screens, Widgets, Bloc/Cubit State Management |
<details>
<summary>📂 View Full Project Structure</summary>

```
📦 lib
 ├── 📄 bloc_observer.dart
 ├── 📄 firebase_options.dart
 ├── 📄 main.dart
 │
 ├── 📂 bindings
 ├── 📂 constants
 ├── 📂 controllers
 │
 ├── 📂 core
 │   ├── 📂 constants
 │   ├── 📂 error
 │   ├── 📂 extensions
 │   ├── 📂 network
 │   ├── 📂 strings
 │   ├── 📂 utils
 │   │   ├── 📂 Localization
 │   │   ├── 📂 styles
 │   │   └── 📂 theme
 │   └── 📂 widgets
 │
 ├── 📂 data
 │   ├── 📂 cache
 │   ├── 📂 models
 │   └── 📂 repository
 │
 ├── 📂 features
 │   ├── 📂 auth
 │   │   ├── 📂 data
 │   │   └── 📂 presentation
 │   │       ├── 📂 blocs
 │   │       ├── 📂 pages
 │   │       └── 📂 widgets
 │   │
 │   ├── 📂 khatma
 │   │   ├── 📂 data
 │   │   ├── 📂 domain
 │   │   └── 📂 presentation
 │   │       ├── 📂 blocs
 │   │       ├── 📂 pages
 │   │       └── 📂 widgets
 │   │
 │   ├── 📂 on_boarding
 │   │   └── 📂 presentation
 │   │
 │   ├── 📂 radio
 │   │   ├── 📂 data
 │   │   ├── 📂 domain
 │   │   └── 📂 presentation
 │   │       ├── 📂 blocs
 │   │       └── 📂 pages
 │   │
 │   └── 📂 sebha
 │       ├── 📂 pages
 │       └── 📂 widgets
 │
 ├── 📂 handlers
 ├── 📂 pages
 ├── 📂 routes
 ├── 📂 services
 │   └── 📂 audio
 ├── 📂 utils
 │   ├── 📂 dialogs
 │   └── 📂 sheets
 ├── 📂 views
 └── 📂 widgets
```

</details>

---

## 📸 Screenshots

<table>
  <tr>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Omarsalama2001/islamina_demo/main/screenshot-1772626258547-portrait.png" width="220"/>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Omarsalama2001/islamina_demo/main/screenshot-1772626320212-portrait.png" width="220"/>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Omarsalama2001/islamina_demo/main/screenshot-1772626361798-portrait.png" width="220"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Omarsalama2001/islamina_demo/main/khatma-portrait.png" width="220"/>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Omarsalama2001/islamina_demo/main/khatma2-portrait.png" width="220"/>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Omarsalama2001/islamina_demo/main/asmaa_allah-portrait.png" width="220"/>
    </td>
  </tr>
  <tr>
    <td align="center" colspan="3">
      <img src="https://raw.githubusercontent.com/Omarsalama2001/islamina_demo/main/radio-portrait.png" width="220"/>
    </td>
  </tr>
</table>

---

## 🔗 Related Projects

<table>
  <tr>
    <td align="center" width="100%">
      <h3>📻 Quran Radio Backend</h3>
      <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
      <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
      <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white"/>
      <br/><br/>
      <p>
        A dedicated <strong>FastAPI</strong> backend that powers the Quran Radio feature,
        providing live streaming from the most famous Islamic radio stations
        around the world 🌍
      </p>
      <a href="https://github.com/Omarsalama2001/islamina1">
        <img src="https://img.shields.io/badge/View_Backend_Repo-181717?style=for-the-badge&logo=github&logoColor=white"/>
      </a>
      &nbsp;
      <a href="https://islamina1-68jbw7rmy-omarsalama2001s-projects.vercel.app/?vercelToolbarCode=nb7OGz7VpUfDpfF">
        <img src="https://img.shields.io/badge/Live_API-success?style=for-the-badge&logo=vercel&logoColor=white"/>
      </a>
    </td>
  </tr>
</table>

---
## 🔒 Source Code

> 🔒 Source code is private.
> Feel free to [contact me](mailto:omarrsalama90111@gmail.com) for more details.

---

## 📬 Contact

<p align="left">
  <a href="mailto:omarrsalama90111@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://www.linkedin.com/in/0marsalama">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://github.com/Omarsalama2001">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
</p>
