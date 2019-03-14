# MQTT Template
This is a standard C++ template that is intended to be used with MQTT and Node-Red and run on an ESP8266 MCU.

My Node-Red server uses the node-red-contrib-blynk-ws plug-in to provide Blynk integration. https://www.npmjs.com/package/node-red-contrib-blynk-ws

However, this template also allows the ESP device to communicate directly with Blynk if needed.
I do not recommend using direct Blynk integration in this way in most situations, but it does allow devices to still be controlled if the MQTT/Node-Red server(s) are down, but internet access is still available. This could allow emergency control of devices in this very narrow set of circumstances.
The direct Blynk integration is deactivated by default, and is activated by un-commenting the #define UseBlynk statement.
