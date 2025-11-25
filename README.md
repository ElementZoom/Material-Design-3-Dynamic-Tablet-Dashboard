# Material-Design-3-Dynamic-Tablet-Dashboard
A modern Home Assistant dashboard built on Material Design 3 (MD3) principles, featuring dynamic colors, transparent and adaptive card layouts, and a sleek, clean UI for an elegant smart home experience.

This comprehensive dashboard unifies control and monitoring for **lights, switches, temperature and humidity sensors, rainfall, wind, UV index, radar, weather forecasts, alarms, Hue scenes, cameras, heat pumps, door and window sensors, and irrigation control** - all presented in one cohesive, visually refined interface designed for both functionality and aesthetic harmony.

[_The v4.0.0_](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/releases/tag/v.4.0.0) major update introduces a significantly more modular system across most cards, making customization far easier than before. Previously, I had to manually adjust large portions of the dashboard to fit their setup. Thanks to the new streamline card architecture, much of the backend complexity has been consolidated. You can now map your entities directly through the UI, reducing setup time and improving flexibility. You can check all the [streamline_templates](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/streamline_templates%20collection) I've used in the dashboard.

In addition to this core upgrade, the update also includes several quality-of-life improvements: a new media player on the overview page, refined layout adjustments for cleaner organization, and expanded use of pop-up cards to keep the interface tidy and intuitive.

# ✨ Features

**🎨 MD3 Theme Engine**

Unlock unlimited color combinations with a simple color picker - thanks to the amazing work of Material You Theme repository.

**👥 Per-User Styling**

Each family member can have their own unique style and colors. Perfect for customizing your phone, tablets, and shared devices.

**💡Community Inspired**

Several cards are inspired by the incredible work of others in the Home Assistant community. Credit will be detailed below.

# 🖼️ Dashboard Walkthrough

**Overview Page**

<img width="1920" height="785" alt="1" src="https://github.com/user-attachments/assets/abcd92ff-6d16-4d35-8858-5db24731aa07" />

**Page Description**

The Overview page serves as the central hub for monitoring and controlling most of my smart devices. At the top, it displays a [personalized greeting](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20greeting) along with the current time, weather conditions, wind speed, and the day’s high and low temperatures.

To the right, there are dedicated [Climate and Irrigation tabs](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Climate%20and%20Irrigation%20Tabs) for managing the thermostat and sprinkler systems. Below them, I have a [Media Card](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Media%20Card), [Calendar](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Calendar), and [Alarmo, with a notification chip for quick alerts](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Alarmo%20%26%20Notificaton%20Chip). When no media is playing, the media card switches back to calendar and backyard camera.

Next, the dashboard features [Room Cards](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Room%20Cards) that provide quick access to thermostat controls, lighting toggles, and the current count of open doors or windows.

Finally, the main page includes four [live camera feeds](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Overview%20Page%20-%20Live%20Camera%20Feeds), streaming in real time for immediate visual monitoring.

***

**Weather Forecast and Notifications Page - Individual Room Page**

<img width="1920" height="782" alt="2" src="https://github.com/user-attachments/assets/55bd537a-e4e4-43d5-bf9b-5b26c210539a" />

**Weather - Notification page** combines all my weather information and notifications in one place for quick status updates and alerts.

On the notifications side, I use a variety of conditional cards powered by [timers](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Notification%20Page%20-%20Timers) and booleans to make alerts appear only when needed - for example, reminders like “wash duvet”, notifications when the sprinklers are running, or warnings about an open door.

The weather section is designed to be clean and informative. Certain cards - like weather warnings, earthquake alerts, and volcano warnings - remain hidden unless there’s an active event (depending on your local integration). The rest of the display includes [detailed weather data](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Notification%20Page%20-%20Weather%20Tab), rainfall, UV index, wind conditions, lunar information, and a live radar map, giving me a complete view of current and upcoming conditions.


**Individual room page** provides detailed controls and status information specific to that space. At the top, it displays the [current temperature, room presence, and the last seen timestamp](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Individual%20Room%20Page%20-%20Room%20Summary) from the occupancy sensor.

Below that, there are [light controls](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Individual%20Room%20Page%20-%20Lights%20%26%20Switch%2C%20including%20navigation%20and%20script), including both slider and button cards, allowing for easy brightness adjustment and quick toggling.

Next to the lighting section, there’s a [Climate Control panel](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Individual%20Room%20Page%20-%20Climate%20Card) that lets me manage the room’s temperature settings, select operation modes, and view the thermostat’s daily runtime. It also shows the current humidity level for that room, including how long the runtime of the climate for the day.

On the right side, two conditional cards appear only when a [door or window is open](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Individual%20Room%20Page%20-%20Open%20Door%20and%20Open%20Windows), helping highlight important changes at a glance.

Finally, a [Media Card](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Individual%20Room%20Page%20-%20Media%20Card) sits inside the pop up card, providing quick access to audio or video playback within the room.

***

**Hue Scene Page**

<img width="1920" height="688" alt="3" src="https://github.com/user-attachments/assets/756ed1c8-b223-40ce-8fb6-965961c785f8" />

**Page Description**

I’ve always loved Philips Hue, but instead of using their bridge, I connect my lights directly through Zigbee2MQTT (Z2M). To recreate the familiar Philips Hue app experience, I use the [hass-scene_preset](https://github.com/Hypfer/hass-scene_presets) integration from HACS, which lets me simulate [Hue’s scene](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Hue%20Page%20-%20Scene%20Example) controls and build my own [room selector](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Hue%20Page%20-%20Room%20Selector).

All of this comes together thanks to the incredible work of the Hypfer - the mainainer of hass-scene_preset, along with a combination of automations, scripts, input_selects, and booleans that make the whole setup seamless.

***

**Camera Page - Timeline and Alarm Page**

<img width="1920" height="710" alt="4" src="https://github.com/user-attachments/assets/39c4442e-7669-4ce0-bbbd-e45829868649" />

**Page Description**

I like having all my [cameras](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Camera%20Page%20-%20Example) displayed together on a dedicated page. There are six cameras around the house, and this page gives me a complete live view of them all in one place.

At the top, there are buttons that let me toggle vehicle and person detection automations. Beneath each camera feed, I’ve added light controls, allowing quick adjustments to the nearby lighting directly from the same view.

I also have my Alarmo integration panel, which can be accessed by clicking the Alarmo button on the Overview page. Right next to it, I display the 10 most recent recorded events, each automatically described by LLM Vision - adding a smart, futuristic touch to the camera setup.

***
**Server - Irrigation Page**

<img width="1920" height="692" alt="5" src="https://github.com/user-attachments/assets/fe3d8e1e-c3cd-40b2-a29d-c83c776d5743" />

The **Server Page** is where I monitor the health and performance of my smart home system. I’m running Home Assistant OS (HAOS) on a mini PC through Proxmox, which is fully integrated into Home Assistant for live monitoring.

This page tracks key [system metrics](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Server%20Page%20-%20Proxmox%20and%20HAOS%20overview) such as memory usage, CPU temperature, network activity, and [device battery levels](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Server%20Page%20-%20Battery%20Overview) (highlighting any that drop below 60%). It gives me a quick overview of my server’s status and connected devices at a glance.

The **Irrigation Page** manages my sprinkler system and garden monitoring. I use two Sonoff Smart Valves to control water flow to the sprinklers, supported by several soil sensors that track both temperature and moisture levels.

To visualize performance, I’ve built a [custom graph](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Irrigation%20Page%20-%20Backyard%20Example) showing water flow trends, and I’ve automated irrigation timers through a combination of automations and scripts, making the watering system efficient and fully autonomous.


***

**Calendar Page**

<img width="1920" height="685" alt="6" src="https://github.com/user-attachments/assets/2ff962e8-c1b1-44b6-bb53-45479d7ec79e" />

**Page Description**

The [Calendar Page](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Calendar%20Page%20-%20Day%20offset%200%20example) provides a full view of my appointments, events, and schedules in one place. It’s a dedicated page that pulls in data from my linked calendars, giving me an easy way to stay on top of upcoming tasks and daily plans right within Home Assistant.

**Extra Cards**

<img width="575" height="268" alt="Lock Example" src="https://github.com/user-attachments/assets/e60d4530-c2da-470d-a95c-23bda4c0ade9" />

Above is an example of [lock card](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Lock%20Card%20Example).

<img width="511" height="372" alt="Scene Example" src="https://github.com/user-attachments/assets/75f01d54-5aad-4bdb-8402-3d389e2ed49d" />

The above is [scene example](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Scene%20Card%20Example) card with mushroom entity card.

<img width="574" height="450" alt="Cover Example" src="https://github.com/user-attachments/assets/3b7a1a29-b637-4307-8250-c5971fa0be59" />

And last one, is a [cover card](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/Curtain%20Card%20Example) example.

# 🚀 Requirements / Dependencies

Card Related Stuffs:
- [Alarmo Card](https://github.com/nielsfaber/alarmo-card)
- [Apex Charts Card](https://github.com/RomRider/apexcharts-card?tab=readme-ov-file#series-options)
- [Bubble Card](https://github.com/Clooos/Bubble-Card)
- [Button-Card](https://github.com/custom-cards/button-card)
- [Calendar Card Pro](https://github.com/alexpfau/calendar-card-pro)
- [LLM Vision Card](https://github.com/valentinfrlch/llmvision-card)
- [Mini-Graph-Card](https://github.com/kalkih/mini-graph-card)
- [Mushroomn](https://github.com/piitaya/lovelace-mushroom)
- [Navbar Card](https://github.com/joseluis9595/lovelace-navbar-card)
- [Simple Swipe Card](https://github.com/nutteloost/simple-swipe-card)
- [Simple Tabs Card](https://github.com/agoberg85/home-assistant-simple-tabs)
- [Timer Bar Card](https://github.com/rianadon/timer-bar-card)
- [Web RTC Camera](https://github.com/AlexxIT/WebRTC)
- [Week Planner Card](https://github.com/FamousWolf/week-planner-card)

Weather Related:
- [Lunar Phase Card](https://github.com/ngocjohn/lunar-phase-card)
- [Lunar Phase Integration](https://github.com/ngocjohn/lunar-phase)
- [World's Air Quality Index](https://www.home-assistant.io/integrations/waqi/)
- [Weather Card Extended](https://github.com/Thyraz/weather-forecast-extended) - new in v3.3.0
- [Clock Weather Card HUI Icons](https://github.com/pkissling/clock-weather-card)

Theming / ETC:
- [Auto-Entities](https://github.com/thomasloven/lovelace-auto-entities)
- [Card-Mod](https://github.com/thomasloven/lovelace-card-mod)
- [Config Template Card](https://github.com/iantrich/config-template-card)
- [Kiosk Mode](https://github.com/maykar/kiosk-mode)
- [Layout-Card](https://github.com/thomasloven/lovelace-layout-card)
- [Lovelace Material Components](https://github.com/giovannilamarmora/lovelace-material-components)
- [Material Symbols](https://github.com/beecho01/material-symbols)
- [Material You Theme](https://github.com/Nerwyn/material-you-theme)
- [Material You Utilities](https://github.com/Nerwyn/material-you-utilities)
- [My Cards Bundle](https://github.com/AnthonMS/my-cards)
- [Paper Buttons Row](https://github.com/jcwillox/lovelace-paper-buttons-row)
- [Stack In Card](https://github.com/custom-cards/stack-in-card)
- [Scene Presets](https://github.com/Hypfer/hass-scene_presets)
- [Streamline Card](https://github.com/brunosabot/streamline-card)
- [Vertical Stack In Card](https://github.com/ofekashery/vertical-stack-in-card)

# Installation

- I recommend you to save all of the [streamline_templates](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/assets/streamline_templates%20collection) I've created and to remove the one you don't end up using.
- Choose which card that you want to adapt to your installation by clicking the hyperlink provided in the description above.
- Install the required HACS components (such as simple swipe card, stack-in-card, popup-card, etc. - see your setup for what’s needed).
- To unlock the full functionality (like weather icons, notification counts, and more), you’ll need to add the corresponding [sensors](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/tree/main/template%20sensor) to your config.
- For the Hue scene, you'll need to have the automation, scripts, input boolean, input text, and input number in your system that you can find in [hue asset folder](https://github.com/ElementZoom/Material-Design-3-Dynamic-Mobile-Dashboard/tree/main/hue%20asset). For the images, you can get them from [here](https://github.com/Hypfer/hass-scene_presets/blob/master/custom_components/scene_presets/assets/Readme.md).
- Apply the MD3 theme and select your preferred colors. It is accessible from Overview page > More > Theme Icon

<img width="1393" height="839" alt="image" src="https://github.com/user-attachments/assets/2392b080-0671-42ac-bc3c-930f0ff4246d" />

- Select the Transparent option in Card Type to get the wide-system transparent cards
  
<img width="556" height="326" alt="image" src="https://github.com/user-attachments/assets/19d19eb5-558c-40fe-ba6e-dd186c2af7b4" />

- Enjoy your personalized dynamic tablet dashboard! 🎉

# 📚 Credits

This project builds upon the work of:
- Nerwyn – [Material You Theme](https://github.com/Nerwyn/material-you-theme) & [Material You Utilities](https://github.com/Nerwyn/material-you-utilities)
- [MySmartHome](https://www.youtube.com/@My_Smart_Home) - for the new tabs button, button cards styling, sliders, etc
- Other community members who kindly shared their cards
- [Background Creator](https://www.pexels.com/photo/a-blurry-background-7640905)

# 💖 Support My Work  

If you want to hire me to make your personal dashboard, you can hit me up on one of these social media platforms below:
- [Discord](https://discord.gg/5tVugEbd)
- Email at  _reynaldi.sutrisno.rs16@gmail.com_
- [Reddit](https://www.reddit.com/u/ElementZoom/s/dr4NN0mTtj)
- [Facebook](https://www.facebook.com/profile.php?id=61578092475703)

Or you can support me on [Ko-fi](https://ko-fi.com/ElementZoom).
Your support helps me keep creating and sharing more awesome open-source tools! Thank you for being part of this journey 🚀
