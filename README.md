# 💡 Presence-Based Lighting Blueprint (Simplified)

This Home Assistant blueprint automates lighting based purely on presence detection.  
It’s designed to provide responsive lighting that turns on when someone enters a room and turns off after a configurable delay, depending on how long presence was active.

---

## ✨ Features

- Turns on lights at a configurable brightness when presence is detected  
- Automatically turns off lights after a delay based on how long the room was occupied  
- No helpers required — all logic is handled internally  
- Easy setup via Home Assistant’s UI

---

## 🧰 Requirements

To use this blueprint, you need:

- A presence sensor (`binary_sensor` with `occupancy` device class)  
- A light entity to control  

✅ No `input_select` or `input_datetime` helpers are needed.

---

## ⚙️ Configuration

When creating an automation from this blueprint, you’ll be asked to:

- Select the presence sensor for the room  
- Choose the light entity to control  
- Set the brightness level  
- Define delay times for different durations of presence:
  - Short (<1 min)
  - Medium (<5 min)
  - Long (<10 min)
  - Extended (>10 min)

---

## 🔗 Import Blueprint

For help on how to import a blueprint, check the official Home Assistant guide:  
👉 [Using Blueprints in Home Assistant](https://www.home-assistant.io/docs/automation/using_blueprints/#importing-blueprints)
