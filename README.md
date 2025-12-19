# home-assistant-blueprints

# Scheduled Outlet Blueprint for Home Assistant

This Home Assistant automation blueprint turns a power outlet **on and off on a configurable schedule**, with:

- Two separate time sets
- Custom **on/off times**
- Configurable **date ranges**
- Specific **days of the week**
- Recovery behavior after **Home Assistant restarts**

The outlet **defaults to ON**, and is only powered OFF during matching time/date windows.

---

## 📥 How to Import the Blueprint

Click this link to import the blueprint directly into Home Assistant:

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?repository_url=https://raw.githubusercontent.com/tomc-ut/home-assistant-blueprints/main/blueprints/automation/tomc-ut/scheduled_outlet_blueprint.yaml)

Or paste this URL in your browser:

https://my.home-assistant.io/redirect/blueprint_import/?repository_url=https://raw.githubusercontent.com/tomc-ut/home-assistant-blueprints/main/blueprints/automation/tomc-ut/scheduled_outlet_blueprint.yaml

### 📄 Manual Import (copy/paste)
If you want to paste the blueprint address directly into **Settings → Automations & Scenes → Blueprints → Import Blueprint**, use this URL as the **Blueprint Address**:

```
https://raw.githubusercontent.com/tomc-ut/home-assistant-blueprints/main/blueprints/automation/tomc-ut/scheduled_outlet_blueprint.yaml
```

Steps:
1. In Home Assistant, open **Settings → Automations & Scenes → Blueprints → Import Blueprint**.
2. Paste the Blueprint Address above into the **Blueprint address** field.
3. Click **Preview** (if available), then **Import**.

---

## 🛠 How to Use

1. Import the blueprint (see above)
2. Create a new automation using this blueprint
3. Configure:
   - The outlet switch entity
   - Two **date ranges**
   - Two pairs of **on/off times**
   - **Days of the week** for each time set
   - (Optional) **Temperature guardrails**: pick a temperature sensor, choose above/below mode, set ON/OFF thresholds, and select °F or °C

---

## 💡 Example Use Case

Turn off a smart plug during daytime hours (e.g., 9am–5pm) on weekdays, but only between June 1 and September 30.

---

## 📄 License

MIT License — see [LICENSE](LICENSE)

---

## 🧾 Changelog

- **1.1.0**
  - Added optional temperature guardrails (sensor selection, Fahrenheit/Celsius choice, above/below mode, and ON/OFF hysteresis thresholds).
  - Added periodic checks and integrated temperature logic with the schedule to keep the outlet in the correct state.
