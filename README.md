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

### Simple Switch Card

### Room Navigation Card
![A room navigation card image](https://i.imgur.com/GxmT4mV.png)

### Vacuum Status Card

### Slider Card
