# Cool Puck

Cool Puck is a small, self-contained device designed to help decide when to open or close a window based on indoor conditions and the weather outside.

The device uses a ring of LEDs to display a simple directional recommendation: open the window or close it. The goal is to turn information about indoor and outdoor conditions into a glanceable, practical suggestion.

## How It Works

Cool Puck combines local environmental measurements with weather information:

- **Indoor temperature:** Measured locally using a 1-Wire temperature sensor.
- **Outdoor conditions:** Retrieved over Wi-Fi from a weather service.
- **Window state:** A sensor can report whether the window is open or closed.
- **Scheduling:** A real-time clock supports scheduled and predictive guidance.
- **Display:** Fifteen white LEDs behind a blue lens form the visual indicator.

The intent is to consider more than just the current temperature. Forecast conditions and timing can help determine whether opening or closing a window will improve indoor comfort.

Humidity is a possible extension. If included, absolute humidity or dew point may be more useful than relative humidity when comparing indoor and outdoor air.

## Hardware

The design is based on an ESP32-class microcontroller and a custom PCB.

Current design considerations include:

- ESP32-S3 or a compact ESP32-based development board
- 1-Wire temperature sensing
- LED control using a TLC59282 driver
- DS1302 real-time clock
- Window-state sensing
- Wi-Fi connectivity for weather information

These are design candidates, not a finalized bill of materials.

## Project Status

Cool Puck is currently in the hardware design stage.

- A schematic exists and needs revision.
- A PCB layout exists and needs revision.
- Component selection and hardware architecture are still being refined.
- No completed prototype or validated firmware is available yet.

The current target is to have the project ready for summer 2027.

## Project Direction

The design goal is a compact, unobtrusive device that provides useful guidance without requiring someone to check an app or interpret a weather forecast.

The project is intentionally focused: provide a simple recommendation based on conditions that matter for deciding when to ventilate a space.
