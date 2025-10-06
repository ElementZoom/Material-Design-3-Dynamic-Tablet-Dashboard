# Material-Design-3-Dynamic-Tablet-Dashboard
A modern Home Assistant dashboard built on Material Design 3 (MD3) principles, now optimized for tablets. It features a dynamic, transparent, and adaptive card layout with a sleek, clean UI for an elegant smart home experience. This tablet dashboard brings together lights, switches, temperature and humidity, rainfall, wind, weather forecasts, alarmo, cameras, heat pumps, hue scenes, door/window sensors, and more—all in one cohesive design adapted from the mobile version.

# ✨ Features

**🎨 MD3 Theme Engine**

Unlock unlimited color combinations with a simple color picker — thanks to the amazing work of Material You Theme repository.

**👥 Per-User Styling**

Each family member can have their own unique style and colors. Perfect for customizing your phone, tablets, and shared devices.

**📱 UI Components**

- Tab Navigations
- Light button sliders
- Other custom buttons
- Waterfall temp/humidity graphs
- Pop-up cards
- Tabs & swipe cards
- Expanders
- Gesture navigation

**💡Community Inspired**

Several cards are inspired by the incredible work of others in the Home Assistant community. Credit will be detailed below.

**🖼️ Screenshots**

<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/680e75f5-a237-47fd-a77a-1bf50be800c5" />

<img width="1920" height="1080" alt="6" src="https://github.com/user-attachments/assets/8f0b4cc7-22f3-467f-ae4f-b8b2badbf9a8" />

<img width="1920" height="1080" alt="7" src="https://github.com/user-attachments/assets/e3c281a4-f232-4dfd-8f63-827dec6dbb0f" />


# 🚀 Requirements / Dependencies

- [Advanced Camera Card](https://github.com/dermotduffy/advanced-camera-card)
- [Alarmo](https://github.com/nielsfaber/alarmo)
- [Alarmo Card](https://github.com/nielsfaber/alarmo-card)
- [Apex Charts Card](https://github.com/RomRider/apexcharts-card?tab=readme-ov-file#series-options)
- [Auto-Entities](https://github.com/thomasloven/lovelace-auto-entities)
- [Bubble Card](https://github.com/Clooos/Bubble-Card)
- [Button-Card](https://github.com/custom-cards/button-card)
- [Calendar Card Pro](https://github.com/alexpfau/calendar-card-pro)
- [Card-Mod](https://github.com/thomasloven/lovelace-card-mod)
- [Clock Weather Card HUI Icons](https://github.com/pkissling/clock-weather-card)
- [Config Template Card](https://github.com/iantrich/config-template-card)
- [Decluttering Card](https://github.com/custom-cards/decluttering-card)
- [Expander-Card](https://github.com/MelleD/lovelace-expander-card)
- [Home Assistant Swipe Navigation](https://github.com/zanna-37/hass-swipe-navigation)
- [Horizontal Waterfall History Card](https://github.com/sxdjt/horizontal-waterfall-history-card)
- [Kiosk Mode](https://github.com/maykar/kiosk-mode)
- [Layout-Card](https://github.com/thomasloven/lovelace-layout-card)
- [Local Conditional Card](https://github.com/PiotrMachowski/Home-Assistant-Lovelace-Local-Conditional-card)
- [Material You Theme](https://github.com/Nerwyn/material-you-theme)
- [Material You Utilities](https://github.com/Nerwyn/material-you-utilities)
- [MetService New Zealand Weather](https://github.com/ciejer/metservice-weather)
- [Mini-Graph-Card](https://github.com/kalkih/mini-graph-card)
- [Mushroomn](https://github.com/piitaya/lovelace-mushroom)
- [My Cards Bundle](https://github.com/AnthonMS/my-cards)
- [Paper Buttons Row](https://github.com/jcwillox/lovelace-paper-buttons-row)
- [Scene Presets](https://github.com/Hypfer/hass-scene_presets)
- [Simple Swipe Card](https://github.com/nutteloost/simple-swipe-card)
- [Simple Tabs Card](https://github.com/agoberg85/home-assistant-simple-tabs) - new in v3.0.0
- [Stack In Card](https://github.com/custom-cards/stack-in-card)
- [Timer Bar Card](https://github.com/rianadon/timer-bar-card)
- [Vertical Stack In Card](https://github.com/ofekashery/vertical-stack-in-card)
- [Web RTC Camera](https://github.com/AlexxIT/WebRTC) - new in v3.0.0
- [World's Air Quality Index](https://www.home-assistant.io/integrations/waqi/)

# Installation

- Create a blank dashboard to start fresh (optional) or copy some part of the codes or full codes from  [full_YAML](https://github.com/ElementZoom/Material-Design-3-Dynamic-Tablet-Dashboard/blob/main/full_yaml) into your Home Assistant dashboard.
- Install the required HACS components (such as simple swipe card, stack-in-card, popup-card, etc. — see your setup for what’s needed).
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
- Newryn – [Material You Theme](https://github.com/Nerwyn/material-you-theme) & [Material You Utilities](https://github.com/Nerwyn/material-you-utilities)
- [MySmartHome](https://www.youtube.com/@My_Smart_Home) - for the new tabs button, button cards styling, sliders, etc
- Other community members who kindly shared their cards
- [Background Creator](https://www.pexels.com/photo/a-blurry-background-7640905)

# 💖 Support My Work  

If you want to hire me to make your personal dashboard, you can hit me up in [Reddit](https://www.reddit.com/u/ElementZoom/s/dr4NN0mTtj)

Or you support me on [Ko-fi](https://ko-fi.com/ElementZoom).  
Your support helps me keep creating and sharing more awesome open-source tools! ✨  

Thank you for being part of this journey 🚀
