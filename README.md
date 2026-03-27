# Quran-TV-OORO
A lightweight, hosted web application for Holy Quran recitation, optimized for Smart TV

## 🚀 Key Features

* **TV-Optimized UI:** High-contrast design and large typography for comfortable reading from a distance (3+ meters).
* **Spatial Navigation:** Full support for D-Pad (Arrow keys) and OK/Enter buttons, ensuring a smooth experience without a mouse.
* **Real-time Streaming:** Integration with the [Quran.com API](https://quran.com/developers) for high-quality audio recitations.
* **Media Controls:** Dedicated Play, Pause, and Stop functionality mapped to both on-screen buttons and hardware remote keys.


## 🛠️ Technical Stack

* **Frontend:** HTML5, CSS3 (Flexbox/Grid), Vanilla JavaScript.
* **API:** Quran.com V4 API.
* **Target Environments:** * Smart TV Browsers (Chromium-based & WPE WebKit).
    * RDK (Reference Design Kit) Platforms.
    * Linux-based

## 📺 How to Use on Your TV

### ⚠️ Integration Steps (For Developers)

To add the **OORO Quran Kareem** app to your TV's home screen launcher, follow these steps:

#### **1. Connect to the TV**
Establish a connection to the TV through a **Serial Debugger** (UART) or via **SSH**.

#### **2. Access the Configuration**
Open the home screen applications configuration file using the `vi` editor:
```bash
vi /data/ooro/homeScreenApps.json
```

#### Add the following JSON object into the homeScreenApps.json file:
```
  {
                    "appName": "OORO Quran Kareem",
                    "url": "https://ahmadabddallah.github.io/Quran-TV-OORO/",
                    "position_x": 10,
                    "position_y": 1,
                    "res_x": 1280,
                    "res_y": 720
  }
```
