# Diagram
{
  "version": 1,
  "author": "Anderson Costa",
  "editor": "wokwi",
  "parts": [
    { "type": "wokwi-pi-pico", "id": "pico", "top": 243.95, "left": 79.76, "attrs": {} },
    { "type": "wokwi-servo", "id": "servo1", "top": 87.09, "left": 21.27, "attrs": {} },
    {
      "type": "wokwi-led",
      "id": "led1",
      "top": 76.21,
      "left": 51.48,
      "attrs": { "color": "blue" }
    },
    {
      "type": "wokwi-led",
      "id": "led2",
      "top": 161.21,
      "left": 53.1,
      "attrs": { "color": "red" }
    }
  ],
  "connections": [
    [ "pico:GP0", "servo1:PWM", "cyan", [ "h-100", "v-9" ] ],
    [ "pico:GND.1", "servo1:GND", "black", [ "h-136", "v-2" ] ],
    [ "pico:3V3", "servo1:V+", "red", [ "h20", "v-83", "h-211", "v-13" ] ],
    [ "led1:C", "pico:GND.1", "yellow", [ "v2", "h-122", "v203" ] ],
    [ "led2:C", "pico:GND.1", "orange", [ "v0", "h-124", "v120" ] ],
    [ "led1:A", "pico:GP1", "lime", [ "v7", "h-125", "v-1" ] ],
    [ "led2:A", "pico:GP2", "blue", [ "v5", "h-122", "v-1" ] ]
  ],
  "dependencies": {}
}
