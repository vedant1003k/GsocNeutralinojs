# Neutralinojs + React Starter

This repository is a starter template for building a **Neutralinojs** application with **React** as the frontend library. It allows you to create lightweight cross-platform desktop applications using web technologies.

## 📌 Features
- 🚀 **Neutralinojs** for lightweight desktop applications
- ⚛️ **React** for a modern frontend
- 🔥 **Hot Module Reloading (HMR)** for fast development
- 📁 **Filesystem API** access with Neutralinojs
- 🛠️ **Developer Tools** enabled for debugging

## 📦 Installation

### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/vedant1003k/GsocNeutralinojs.git
cd Demo
```

### **2️⃣ Initializing native API with @neutralinojs/lib**
```sh
cd react-src
npm install
npm install @neutralinojs/lib
```

## 🔧 Configuration

### **📂 Update `neutralino.config.json`**
Modify the configuration file to set the document root and add permissions for using the filesystem API.

```json
{
  "documentRoot": "/react-src/build/",
  "nativeAllowList": [
    "app.*",
    "filesystem.readDirectory"
  ],
  "modes": {
    "window": {
      "icon": "/react-src/public/logo192.png"
    }
  },
  "cli": {
    "resourcesPath": "/react-src/build/",
    "frontendLibrary": {
        "patchFile": "/react-src/public/index.html",
        "devUrl": "http://localhost:3000",
        "projectPath": "/react-src/",
        "initCommand": "npm install",
        "devCommand": "BROWSER=none npm start",
        "buildCommand": "npm run build"
    }
  }
}
```

## 🚀 Running the Application

### **1️⃣ Build the React App**
```sh
cd react-src
npm run build
cd ..
```

### **2️⃣ Run the Neutralinojs App**
```sh
neu run -- --window-enable-inspector
```

## 🛠 Enabling Hot-Reload
Instead of building after every change, enable Hot Module Reloading (HMR):
```sh
neu run
```
This will start the development server at `http://localhost:3000` with Neutralinojs.

---
Made with ❤️ using **Neutralinojs & React**.






# neutralinojs-minimal

The default template for a Neutralinojs app. It's possible to use your favorite frontend framework by using [these steps](https://neutralino.js.org/docs/getting-started/using-frontend-libraries).

## Contributors

[![Contributors](https://contrib.rocks/image?repo=neutralinojs/neutralinojs-minimal)](https://github.com/neutralinojs/neutralinojs-minimal/graphs/contributors)

## License

[MIT](LICENSE)

## Icon credits

- `trayIcon.png` - Made by [Freepik](https://www.freepik.com) and downloaded from [Flaticon](https://www.flaticon.com)
