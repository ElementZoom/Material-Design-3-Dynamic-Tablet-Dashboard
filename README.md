# Material-Design-3-Dynamic-Tablet-Dashboard
A modern Home Assistant dashboard built on Material Design 3 (MD3) principles, featuring dynamic colors, transparent and adaptive card layouts, and a sleek, clean UI for an elegant smart home experience.

This comprehensive dashboard unifies control and monitoring for **lights, switches, temperature and humidity sensors, rainfall, wind, UV index, radar, weather forecasts, alarms, Hue scenes, cameras, heat pumps, door and window sensors, and irrigation control** - all presented in one cohesive, visually refined interface designed for both functionality and aesthetic harmony.

[v2.0.0](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/releases/tag/v.2.0.0) marks a major update focused on usability, clarity, and performance. This release introduces a guided dashboard walkthrough, refreshed visuals, and several new pages - including irrigation, server, alarmo with camera integration, and a calendar overview. Alongside these additions, the notification center has been reworked for better visibility, and system performance has been optimized for a smoother experience throughout.

# ✨ Features

**🎨 MD3 Theme Engine**

Unlock unlimited color combinations with a simple color picker - thanks to the amazing work of Material You Theme repository.

**👥 Per-User Styling**

Each family member can have their own unique style and colors. Perfect for customizing your phone, tablets, and shared devices.

**💡Community Inspired**

Several cards are inspired by the incredible work of others in the Home Assistant community. Credit will be detailed below.

# 🖼️ Dashboard Walkthrough

**Overview Page**

<img width="1920" height="762" alt="4" src="https://github.com/user-attachments/assets/eb6f0c36-d535-4b06-83d3-7b9a91954747" />


**Page Description**

The Overview page serves as the central hub for monitoring and controlling most of my smart devices. At the top, it displays a personalized greeting along with the current time, weather conditions, wind speed, and the day’s high and low temperatures.

To the right, there are dedicated Climate and Irrigation tabs for managing the thermostat and sprinkler systems. Below them, I have a Media Card, Calendar, and Alarmo (alarm system) components, along with a Notification Chip for quick alerts. When no media is playing, the Media Card automatically switches to display the weather forecast instead.

Next, the dashboard features Room Cards that provide quick access to thermostat controls, lighting toggles, and the current count of open doors or windows.

Finally, the main page includes four live camera feeds, streaming in real time for immediate visual monitoring.

***

**Individual Room Page -  Weather Forecast and Notifications Page**

<img width="1920" height="748" alt="5" src="https://github.com/user-attachments/assets/69c2ec66-c0bd-48c6-8634-e5e2028fc74d" />


**Individual room page** provides detailed controls and status information specific to that space. At the top, it displays the current temperature, room presence, and the last seen timestamp from the occupancy sensor.

Below that, there are light controls, including both slider and button cards, allowing for easy brightness adjustment and quick toggling.

Next to the lighting section, there’s a Climate Control panel that lets me manage the room’s temperature settings, select operation modes, and view the thermostat’s daily runtime. It also shows the current humidity level for that room.

On the right side, two conditional cards appear only when a door or window is open, helping highlight important changes at a glance.

Finally, a Media Card sits below the light controls, providing quick access to audio or video playback within the room.


**Weather - Notification page** combines all my weather information and notifications in one place for quick status updates and alerts.

On the notifications side, I use a variety of conditional cards powered by timers and booleans to make alerts appear only when needed - for example, reminders like “wash duvet”, notifications when the sprinklers are running, or warnings about an open door. Alongside these, I’ve included light and button controls, making it easy to take action directly from the same page.

The weather section is designed to be clean and informative. Certain cards - like weather warnings, earthquake alerts, and volcano warnings - remain hidden unless there’s an active event. The rest of the display includes detailed weather data, rainfall, UV index, wind conditions, lunar information, and a live radar map, giving me a complete view of current and upcoming conditions.

***

**Hue Scene Page**

<img width="1920" height="708" alt="6" src="https://github.com/user-attachments/assets/068869f4-06ed-45db-ae99-ddd1c4ed5a0f" />

**Page Description**

I’ve always loved Philips Hue, but instead of using their bridge, I connect my lights directly through Zigbee2MQTT (Z2M). To recreate the familiar Philips Hue app experience, I use the Hue [Scene Preset](https://github.com/Hypfer/hass-scene_presets) integration from HACS, which lets me simulate Hue’s scene controls and build my own room selector.

All of this comes together thanks to the incredible work of the HACS maintainers, along with a combination of automations, scripts, input_selects, and booleans that make the whole setup seamless.

***

**Camera Page - Timeline and Alarm Page**

<img width="1920" height="785" alt="7" src="https://github.com/user-attachments/assets/e507554f-13ab-4e07-87d1-b723ec8e5c2f" />

**Page Description**

I like having all my cameras displayed together on a dedicated page. There are six cameras around the house, and this page gives me a complete live view of them all in one place.

At the top, there are buttons that let me toggle vehicle and person detection automations. Beneath each camera feed, I’ve added light controls, allowing quick adjustments to the nearby lighting directly from the same view.

I also have my Alarmo integration panel, which can be accessed by clicking the Alarmo button on the Overview page. Right next to it, I display the 10 most recent recorded events, each automatically described by LLM Vision - adding a smart, futuristic touch to the camera setup.

***
**Server - Irrigation Page**

<img width="1920" height="764" alt="8" src="https://github.com/user-attachments/assets/6be92ad4-1f4c-4030-8c45-ceb2d2151572" />

**Page Description**

The **Server Page** is where I monitor the health and performance of my smart home system. I’m running Home Assistant OS (HAOS) on a mini PC through Proxmox, which is fully integrated into Home Assistant for live monitoring.

This page tracks key system metrics such as memory usage, CPU temperature, network activity, and device battery levels (highlighting any that drop below 60%). It gives me a quick overview of my server’s status and connected devices at a glance.

The **Irrigation Page** manages my sprinkler system and garden monitoring. I use two Sonoff Smart Valves to control water flow to the sprinklers, supported by several soil sensors that track both temperature and moisture levels.

To visualize performance, I’ve built a custom graph showing water flow trends, and I’ve automated irrigation timers through a combination of automations and scripts, making the watering system efficient and fully autonomous.


***

**Calendar Page**

<img width="1920" height="756" alt="9" src="https://github.com/user-attachments/assets/f9e1d119-ea56-49ba-a13e-8c217909bc5d" />

**Page Description**

The Calendar Page provides a full view of my appointments, events, and schedules in one place. It’s a dedicated page that pulls in data from my linked calendars, giving me an easy way to stay on top of upcoming tasks and daily plans right within Home Assistant.


# 🚀 Requirements / Dependencies

Card Related Stuffs:
- [Alarmo Card](https://github.com/nielsfaber/alarmo-card)
- [Apex Charts Card](https://github.com/RomRider/apexcharts-card?tab=readme-ov-file#series-options)
- [Clock Weather Card HUI Icons](https://github.com/pkissling/clock-weather-card)
- [Bubble Card](https://github.com/Clooos/Bubble-Card)
- [Button-Card](https://github.com/custom-cards/button-card)
- [Calendar Card Pro](https://github.com/alexpfau/calendar-card-pro)
- [Expander-Card](https://github.com/MelleD/lovelace-expander-card)
- [LLM Vision Card](https://github.com/valentinfrlch/llmvision-card)
- [Mini-Graph-Card](https://github.com/kalkih/mini-graph-card)
- [Mushroomn](https://github.com/piitaya/lovelace-mushroom)
- [Navbar Card](https://github.com/joseluis9595/lovelace-navbar-card)
- [Simple Swipe Card](https://github.com/nutteloost/simple-swipe-card)
- [Simple Tabs Card](https://github.com/agoberg85/home-assistant-simple-tabs)
- [Timer Bar Card](https://github.com/rianadon/timer-bar-card)
- [Web RTC Camera](https://github.com/AlexxIT/WebRTC)
- [Week Planner Card](https://github.com/FamousWolf/week-planner-card)

Theming / ETC:
- [Auto-Entities](https://github.com/thomasloven/lovelace-auto-entities)
- [Card-Mod](https://github.com/thomasloven/lovelace-card-mod)
- [Config Template Card](https://github.com/iantrich/config-template-card)
- [Decluttering Card](https://github.com/custom-cards/decluttering-card)
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
- [Vertical Stack In Card](https://github.com/ofekashery/vertical-stack-in-card)

Weather Related:
- [Lunar Phase Card](https://github.com/ngocjohn/lunar-phase-card)
- [Lunar Phase Integration](https://github.com/ngocjohn/lunar-phase) - new in v3.2.0
- [World's Air Quality Index](https://www.home-assistant.io/integrations/waqi/)

# Installation

- Create a blank dashboard to start fresh (optional) or copy some part of the codes or full codes from  [full_YAML](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/full_yaml) into your Home Assistant dashboard.
- Install the required HACS components (such as simple swipe card, stack-in-card, popup-card, etc. - see your setup for what’s needed).
- You need to adjust the navbar card directory to suit your current dashboard (if you don't start fresh).
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

If you want to hire me to make your personal dashboard, you can hit me up in [Reddit](https://www.reddit.com/u/ElementZoom/s/dr4NN0mTtj) or send me an email at _reynaldi.sutrisno.rs16@gmail.com_

You can also support me on [Ko-fi](https://ko-fi.com/ElementZoom). Your support helps me keep creating and sharing more awesome open-source tools! ✨  

Thank you for being part of this journey 🚀
