# homeassistant-dashboard
This is a template for home assistant dashboards

## Requirements
1. button-card
2. my-slider-v2

## How to install this template?
Just add a whole code from [template.yaml](https://raw.githubusercontent.com/ozeppo/homeassistant-dashboard/main/template.yaml) to a top of a dashboard raw code.

## Cards & how to use them

### Light Card
A simple card for controlling lights.

![A light card image](https://i.imgur.com/9Spio42.png)

In variables setup what you need for your card.

```yaml
type: custom:button-card
template: light-card
variables:
  var_name: Celling
  var_label: Living Room
  var_entity: light.living_room
  var_icon: mdi:lightbulb
```

A option you can set:
```var_name``` - Main header on card
```var_label``` - Second text on card
```var_entity``` - Switch-type entity
```var_icon``` - Icon for a card

### Simple Switch Card

```yaml
type: custom:button-card
template: simple-switch-card
variables:
  var_name: Office Socket
  var_entity: sensor.entity
  var_icon: mdi:power-socket-eu
```

A option you can set:
```var_name``` - Main header on card
```var_entity``` - Entity with a switch option
```var_icon``` - Icon for card

### Room Navigation Card
![A room navigation card image](https://i.imgur.com/GxmT4mV.png)

```yaml
type: custom:button-card
template: room-navigation-card
variables:
  var_name: Living Room
  var_entity: sensor.temperature
  var_icon: mdi:sofa
  var_navigationPath: /lovelace/living-room
  var_color: '#EE4266'
```

A option you can set:
```var_name``` - Main header on card
```var_entity``` - Temperature sensor for card
```var_icon``` - Icon for room
```var_navigationPath``` - Where to navigate when clicking the card
```var_color``` - Color for icon background

### Vacuum Status Card

### Slider Card
