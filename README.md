# Material-Design-3-Dynamic-Tablet-Dashboard
A modern Home Assistant dashboard built on Material Design 3 (MD3) principles, featuring dynamic colors, transparent and adaptive card layouts, and a sleek, clean UI for an elegant smart home experience.

This comprehensive dashboard unifies control and monitoring for **lights, switches, temperature and humidity sensors, rainfall, wind, UV index, radar, weather forecasts, alarms, Hue scenes, cameras, heat pumps, door and window sensors, and irrigation control** - all presented in one cohesive, visually refined interface designed for both functionality and aesthetic harmony.

[_v.6.0.0_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Mobile-Dashboard/releases/tag/v6.0.0) brings several new cards and usability improvements. A new Person Card shows who is home or away, while the current weather card has been streamlined into a single-line layout that still preserves most key information. This release also adds a Location Tracker, Battery Monitoring card for real-time sensor battery status, and a WiFi QR scanner for easy guest network access. Lighting controls have been upgraded with custom button cards to apply transparancy, the Curtain card now uses a custom implementation for better performance, and the Hue scene room selector has been expanded to support more rooms. Additionally, Expander cards help keep rooms organized by allowing sections to be collapsed, and new UI animations enhance visual feedback across the dashboard. This update also fixes animation artifacts and improves responsiveness when changing Hue scenes.

I have also readded the [_full dashboard yaml_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/dashboard.yaml), one of the most requested feature over the communities.

<img width="1458" height="867" alt="Screenshot 2026-03-28 082122" src="https://github.com/user-attachments/assets/c4f590c9-deb2-4d18-a81a-e77a2d19f4b7" />

# ✨ Features

**🎨 MD3 Theme Engine**

Unlock unlimited color combinations with a simple color picker - thanks to the amazing work of Material You Theme repository.

**👥 Per-User Styling**

Each family member can have their own unique style and colors. Perfect for customizing your phone, tablets, and shared devices.

**💡Community Inspired**

Several cards are inspired by the incredible work of others in the Home Assistant community. Credit will be detailed below.

# 🖼️ Dashboard Walkthrough

**Overview Page**

<img width="1450" height="857" alt="Screenshot 2026-03-28 082710" src="https://github.com/user-attachments/assets/a0331aff-e8bd-42fa-8366-dffd0ba34832" />


**Page Description**

The Overview page serves as the central hub for monitoring and controlling most of my smart devices. At the top, it displays a [personalized greeting](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20greeting) along with the current time, weather conditions, wind speed, and the day’s high and low temperatures.

To the right, there are dedicated [_Climate, Toggles, Irrigation, and Hue Scene Tab_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Climate,%20Toggles,%20Irrigation,%20Hue%20Scene%20Tabs) for managing the thermostat, quick toggles,sprinkler systems navigation, and hue scene navigation. Next, there is a [_weather forecast_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Weather%20Forecast) card to show the temperature range for the next 5 days.  [_Calendar_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Calendar), and [_Alarmo, with a notification chip for quick alerts, calendar, music, and camera_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Alarmo%20%26%20Notificaton%20Chip). When no media is playing, the media card switches back to calendar and backyard camera.

Next, the dashboard features [_Room Cards_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Room%20Cards) that provide quick access to thermostat controls, lighting toggles, and the current count of open doors or windows.

Finally, the main page includes four [_live camera feeds_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Live%20Camera%20Feeds), streaming in real time for immediate visual monitoring.

**_Components Used:_**
- [Auto-Entities](https://github.com/thomasloven/lovelace-auto-entities)
- [Button-Card](https://github.com/custom-cards/button-card)
- [Calendar Card Pro](https://github.com/alexpfau/calendar-card-pro)
- [Clock Weather Card HUI Icons](https://github.com/samuelgoodell/clock-weather-card-hui-icons)
- [Config Template Card](https://github.com/iantrich/config-template-card)
- [Mini-Graph-Card](https://github.com/kalkih/mini-graph-card)
- [Mushroom](https://github.com/piitaya/lovelace-mushroom)
- [Paper Buttons Row](https://github.com/jcwillox/lovelace-paper-buttons-row)
- [Simple Swipe Card](https://github.com/nutteloost/simple-swipe-card)
- [Simple Tabs Card](https://github.com/agoberg85/home-assistant-simple-tabs)
- [WebRTC](https://github.com/AlexxIT/WebRTC)

***


**Weather Forecast and Notifications Page**

<img width="1450" height="880" alt="Screenshot 2026-03-28 082323" src="https://github.com/user-attachments/assets/318ff47b-a8e1-438e-8491-8e0a5b79d9ec" />
<img width="1441" height="879" alt="Screenshot 2026-03-28 082354" src="https://github.com/user-attachments/assets/c284876d-e6f8-473b-906b-e7a587b47abd" />


**Weather - Notification page** combines all my weather information and notifications in one place for quick status updates and alerts.

On the notifications side, I use a variety of conditional cards powered by [_timers_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Notification%20Page%20-%20Timers) and booleans to make alerts appear only when needed - for example, reminders like “wash duvet”, notifications when the sprinklers are running, or warnings about an open door.

The weather section is designed to be clean and informative. Certain cards - like weather warnings, earthquake alerts, and volcano warnings - remain hidden unless there’s an active event (depending on your local integration). The rest of the display includes [_detailed weather data_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Notification%20Page%20-%20Weather%20Tab), rainfall, UV index, wind conditions, lunar information, and a live radar map, giving me a complete view of current and upcoming conditions.

**_Components Used:_**
- [Apex Charts Card](https://github.com/RomRider/apexcharts-card?tab=readme-ov-file#series-options)
- [Auto-Entities](https://github.com/thomasloven/lovelace-auto-entities)
- [Button-Card](https://github.com/custom-cards/button-card)
- [Custom Card Features](https://github.com/Nerwyn/custom-card-features)
- [Lunar Phase Card](https://github.com/ngocjohn/lunar-phase-card)
- [Lunar Phase Integration](https://github.com/ngocjohn/lunar-phase)
- [Mushroom](https://github.com/piitaya/lovelace-mushroom)
- [Simple Swipe Card](https://github.com/nutteloost/simple-swipe-card)
- [Simple Tabs Card](https://github.com/agoberg85/home-assistant-simple-tabs)
- [World's Air Quality Index](https://www.home-assistant.io/integrations/waqi/)
- [Weather Card Extended](https://github.com/Thyraz/weather-forecast-extended)

**Individual Room Page**
<img width="1455" height="876" alt="Screenshot 2026-03-28 082134" src="https://github.com/user-attachments/assets/ae7378cc-ecf3-41f2-9347-20f360b30854" />
<img width="1450" height="856" alt="Screenshot 2026-03-28 084440" src="https://github.com/user-attachments/assets/6d2e1c16-c095-4893-8440-293337b2a046" />
<img width="1461" height="856" alt="Screenshot 2026-03-28 093857" src="https://github.com/user-attachments/assets/508f8e8e-01c4-45a0-adf2-224c22f92fcc" />

**Individual room page** provides detailed controls and status information specific to that room. It can show live camera, light, button, and all the other things that we can manipulate in the room.

**_Components Used:_**
- [Material Home Component](https://github.com/giovannilamarmora/lovelace-material-components)
- [Mushroom](https://github.com/piitaya/lovelace-mushroom)
- [WebRTC](https://github.com/AlexxIT/WebRTC)

***

**Hue Scene Page**

<img width="1455" height="871" alt="Screenshot 2026-03-28 082420" src="https://github.com/user-attachments/assets/e40fde10-4cbd-47fd-80fd-00ba951d076e" />
<img width="1453" height="877" alt="Screenshot 2026-03-28 082428" src="https://github.com/user-attachments/assets/63ae85c3-f8fa-4732-9285-d454c62ed977" />

**Page Description**

I’ve always loved Philips Hue, but instead of using their bridge, I connect my lights directly through Zigbee2MQTT (Z2M). To recreate the familiar Philips Hue app experience, I use the [_hass-scene_preset_](https://github.com/Hypfer/hass-scene_presets) integration from HACS, which lets me simulate [Hue’s scene](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Hue%20Page%20-%20Scene%20Example) controls and build my own [_room selector_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Hue%20Page%20-%20Room%20Selector).

All of this comes together thanks to the incredible work of the Hypfer - the mainainer of hass-scene_preset, along with a combination of automations, scripts, input_selects, and booleans that make the whole setup seamless.

**_Components Used:_**
- [Bubble Card](https://github.com/Clooos/Bubble-Card)
- [Button-Card](https://github.com/custom-cards/button-card)
- [Scene Presets](https://github.com/Hypfer/hass-scene_presets)
- [Mushroom](https://github.com/piitaya/lovelace-mushroom)
- [Navbar Card](https://github.com/joseluis9595/lovelace-navbar-card)


***

**Camera Page - Alarm Page**

<img width="1460" height="883" alt="Screenshot 2026-03-28 101230" src="https://github.com/user-attachments/assets/2b72d7b8-fa98-403a-8980-e86d6f440401" />


**Page Description**

I like having all my [_cameras_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Camera%20Page%20-%20Example) displayed together on a dedicated page. There are six cameras around the house, and this page gives me a complete live view of them all in one place.

At the top, there are buttons that let me toggle vehicle and person detection automations. Beneath each camera feed, I’ve added light controls, allowing quick adjustments to the nearby lighting directly from the same view.

I also have my Alarmo integration panel, which can be accessed by clicking the Alarmo button on the Overview page. Right next to it, I display the 10 most recent recorded events, each automatically described by LLM Vision - adding a smart, futuristic touch to the camera setup.

**_Components Used:_**
- [Alarmo Card](https://github.com/nielsfaber/alarmo-card)
- [Mushroom](https://github.com/piitaya/lovelace-mushroom)
- [Simple Tabs Card](https://github.com/agoberg85/home-assistant-simple-tabs)
- [Web RTC Camera](https://github.com/AlexxIT/WebRTC)

***
**Irrigation Page**

<img width="1466" height="882" alt="Screenshot 2026-03-28 101405" src="https://github.com/user-attachments/assets/4b831f50-93a6-4a86-86bb-6b181f42e11e" />

The **Irrigation Page** manages my sprinkler system and garden monitoring. I use two Sonoff Smart Valves to control water flow to the sprinklers, supported by several soil sensors that track both temperature and moisture levels.

To visualize performance, I’ve built a [_custom graph_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Irrigation%20Page%20-%20Backyard%20Example) showing water flow trends, and I’ve automated irrigation timers through a combination of automations and scripts, making the watering system efficient and fully autonomous.

**_Components Used:_**
- [Config Template Card](https://github.com/iantrich/config-template-card)
- [Mushroom](https://github.com/piitaya/lovelace-mushroom)
- [Paper Buttons Row](https://github.com/jcwillox/lovelace-paper-buttons-row)
- [Simple Tabs Card](https://github.com/agoberg85/home-assistant-simple-tabs)


***

**Calendar Page**

<img width="1461" height="884" alt="Screenshot 2026-03-28 101458" src="https://github.com/user-attachments/assets/c66ada28-1ec6-4ee7-861a-df31c71ab0b3" />

**Page Description**

The [_Calendar Page_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Calendar%20Page%20-%20Day%20offset%200%20example) provides a full view of my appointments, events, and schedules in one place. It’s a dedicated page that pulls in data from my linked calendars, giving me an easy way to stay on top of upcoming tasks and daily plans right within Home Assistant.

**_Components Used:_**
- [Calendar Card Pro](https://github.com/alexpfau/calendar-card-pro)

**Extra Cards**

<img width="575" height="268" alt="Lock Example" src="https://github.com/user-attachments/assets/e60d4530-c2da-470d-a95c-23bda4c0ade9" />

Above is an example of [lock card](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Lock%20Card%20Example).

<img width="511" height="372" alt="Scene Example" src="https://github.com/user-attachments/assets/75f01d54-5aad-4bdb-8402-3d389e2ed49d" />

The above is [scene example](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Scene%20Card%20Example) card with mushroom entity card.

<img width="574" height="450" alt="Cover Example" src="https://github.com/user-attachments/assets/3b7a1a29-b637-4307-8250-c5971fa0be59" />

And last one, is a [cover card](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Curtain%20Card%20Example) example.

# Other Components:

Theme / Layout:

- [Material Symbols](https://github.com/beecho01/material-symbols)
- [Material You Theme](https://github.com/Nerwyn/material-you-theme)
- [Material You Utilities](https://github.com/Nerwyn/material-you-utilities)
- [Kiosk Mode](https://github.com/maykar/kiosk-mode)
- [Stack In Card](https://github.com/custom-cards/stack-in-card)
- [Streamline Card](https://github.com/brunosabot/streamline-card)
- [Vertical Stack In Card](https://github.com/ofekashery/vertical-stack-in-card)

# Installation

**For new user:**
- Copy all the code from [_full dashboard yaml_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/dashboard.yaml) to a new dashboard raw configuration editor to jumpstart your experience.
- Install the required HACS components (such as simple swipe card, stack-in-card, popup-card, etc. - see your setup for what’s needed).
- To unlock the full functionality (like weather icons, notification counts, and more), you’ll need to add the corresponding [sensors](https://github.com/ElementZoom/Material-Design-3-Dynamic-Mobile-Dashboard/tree/main/template%20sensor) to your config.
- For the Hue scene, you'll need to have the automation, scripts, input boolean, input text, and input number in your system that you can find in [hue asset folder](https://github.com/ElementZoom/Material-Design-3-Dynamic-Mobile-Dashboard/tree/main/hue%20asset). For the images, you can get them from [here](https://github.com/Hypfer/hass-scene_presets/blob/master/custom_components/scene_presets/assets/Readme.md).
- Apply the MD3 theme and select your preferred colors. It is accessible from Overview page > More > Bucket Fill Icon
- Apply [wallpaper](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/tree/main/wallpaper) (optional)
- Set the companion app to full screen (optional)

**For existing user:**
- Review the [streamline_template](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/streamline_templates%20collection) to see if you want to add / modify the previous version to the new version.
- Choose which card / visuals that you like to be added to your installation by clicking the hyperlink provided in the description above.
- Apply [wallpaper](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/tree/main/wallpaper) (optional)
- Set the companion app to full screen (optional)

# 📚 Credits

This project builds upon the work of:
- Nerwyn – [Material You Theme](https://github.com/Nerwyn/material-you-theme) & [Material You Utilities](https://github.com/Nerwyn/material-you-utilities)
- [MySmartHome](https://www.youtube.com/@My_Smart_Home) - for the new tabs button, button cards styling, sliders, etc
- Other community members who kindly shared their cards

# 💖 Support My Work  

If you want to hire me to make your personal dashboard, you can hit me up on one of these social media platforms below:
- Email at  _reynaldi.sutrisno.rs16@gmail.com_
- [Reddit](https://www.reddit.com/u/ElementZoom/s/dr4NN0mTtj)
- [Facebook](https://www.facebook.com/profile.php?id=61578092475703)

Or you can support me on [Ko-fi](https://ko-fi.com/ElementZoom).
Your support helps me keep creating and sharing more awesome open-source tools! Thank you for being part of this journey 🚀
