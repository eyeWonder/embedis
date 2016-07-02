# Embedis Server - Embedded Dictionary Server

## Examples for ESP8266 WiFi Platform

The Arduino IDE now has the capability to support many different CPU architectures and boards.
These examples are specifically for the ESP8266 WiFi Platform.

## Embedis Servers

    embedis_servers : embedis, web, and telnet servers for ESP8266
    
    This example Arduino IDE sketch for the ESP8266 platform
    (or the Arduino Platform + WiFI Shield Configuration) 
    is used to provide three (3) simultaineous server applications, namely :
    1) Embedis Command Line Interface on Serial (Hardware Serial Monitor)
    2) Web Based Embedis Command Line Interface on Port 80
    3) Telnet Based Embedis Command Line Interface on Port 23

    Any of those Servers can be used to get/set keys in the EEPROM database,
    such as the the WiFi SSID and Passphrase. You no longer need to embed 
    that "data" into your "program"! The EEPROM is persistant, and can be
    used across multiple projects to configure your program setting for
    the specific hardware and network configuration you are using. 
    
    Now, you don't need to recompile your program and reflash your device
    in order to change the device settings anymore. If your ESP8266 WiFi
    doesn't connect, it reverts to an Access Point with a Web Server to allow
    you to change the configuration settings and join another WiFi network.

    We think that this is a much better mechanism for storing settings between projects.
    Once you start using Embedis for your projects, you'll see how quick and easy
    it is to move and reconfigure your devices without needing to recompile 
    and reflash your device firmware just to change a configuration setting.
    Now settings can be changed "on-the-fly" with just a web browser.
    (some settings changes however, will require a restart/reboot to take effect.)

   ====================================================================================== 

    SECURITY CAUTION: (WARNING!)
    These examples demonstrate only simple authentication methods.
    These are not intended to be secure, they are teaching examples only.

    SIMPLE AUTHENTICATION:
    The authentication scheme used here is very, very simple, where the
    default device password is a lowercased base64 function of that 
    devices access point Media Access Control, or Ethernet Hardware Address.
    
    The default device password will be printed out on the Serial Monitor during bootup,
    and should be unique for each device. This is important in a classroom situation
    to keep each student from (accidentally...) accessing/changing their neighbors device.
    
    It is not intended for use in a production environment, where we suggest that 
    encryted keys and values be used, however that is beyond of the scope of this example.
    Embedis itself is transparent, so a more secure implementation would encrypt
    the values (and even the keys themselves) prior to calling Embedis. 
    In this example, all of the keys and values are in unencrypted plain-text, 
    for demonstration, teaching, and debugging purposes.
    
## Contributors

The folks who make this project possible:

 * PatternAgents, LLC
 * Tom Moxon
 * David Turnbull

## Community Supported

[Embedis](https://github.com/thingSoC/embedis) and  [thingSoC](http://www.thingsoc.com) are community supported, you can help by donating to support this work.

<span class="badge-paypal"><a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&amp;hosted_button_id=5NPC24C7VQ89L" title="Donate to this project using Paypal"><img src="https://img.shields.io/badge/paypal-donate-yellow.svg" alt="PayPal donate button" /></a></span>
