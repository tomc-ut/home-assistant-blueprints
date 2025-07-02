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

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?repository_url=https://raw.githubusercontent.com/Gruph/home-assistant-blueprints/main/blueprints/automation/Gruph/scheduled_outlet_blueprint.yaml)

Or paste this URL in your browser:

https://my.home-assistant.io/redirect/blueprint_import/?repository_url=https://raw.githubusercontent.com/Gruph/home-assistant-blueprints/main/blueprints/automation/Gruph/scheduled_outlet_blueprint.yaml

---

## 🛠 How to Use

1. Import the blueprint (see above)
2. Create a new automation using this blueprint
3. Configure:
   - The outlet switch entity
   - Two **date ranges**
   - Two pairs of **on/off times**
   - **Days of the week** for each time set

---

## 💡 Example Use Case

Turn off a smart plug during daytime hours (e.g., 9am–5pm) on weekdays, but only between June 1 and September 30.

---

## 📄 License

MIT License — see [LICENSE](LICENSE)
