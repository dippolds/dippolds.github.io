---
title: "Wireless Network Camera"
date: 2008-03-07 13:18:00 -0500
categories: [Tech]
tags: [Networking, Camera, WiFi, Panasonic]
---

# Panasonic Wireless 802.11b/g Network Camera and Pet Cam (BL-C30A)

These setup notes are adapted from an Amazon user review and were helpful when configuring the camera on a Mac.

## Setup Instructions

1. Plug the camera into AC power and hold down the **reset** pin with a pen.  
   My computer would not recognize the camera until I physically reset it.

2. Make sure the camera switch is set to **Wired**.

3. Connect the camera to your Mac using an Ethernet cable.

4. Temporarily assign your Mac a manual IP address:
   - IP Address: `192.168.0.5`
   - Subnet Mask: `255.255.255.0`

5. Open Safari and connect to:

   ```text
   http://192.168.0.253
````

6. Proceed through setup, but select **No** when asked whether you want to connect the camera to the internet.

7. Re-enter the camera address in Safari:

   ```text
   http://192.168.0.253
   ```

8. Click the **Single** tab to access camera controls.

9. Click the **Setup** tab.

10. Open the **Static IP** configuration page.

11. Disable the Windows auto-setup checkbox.

12. Assign the camera an IP address on your wireless network.

    Example:

    ```text
    192.168.2.253
    ```

13. Enter your router’s gateway address.

    Example:

    ```text
    192.168.2.1
    ```

14. Open the **Wireless** tab.

15. Enter your wireless network SSID exactly as configured.

16. Enter your WEP key and choose the correct key format (ASCII, HEX, etc.).

17. Save the settings.

18. Configure additional settings such as date and time.

19. Disconnect the Ethernet cable.

20. Switch the camera from **Wired** to **Wireless**.

21. Power cycle the camera by unplugging and reconnecting power.

22. Wait for the blinking startup process to finish.
    A solid green light indicates success.

23. Restore your Mac network settings to normal Wi-Fi.

24. Access the camera wirelessly using its assigned IP address.

## Remote Access

Your router blocks incoming internet traffic by default, so the camera will not be accessible externally unless you configure **port forwarding** (also called a virtual server).

Consult your router documentation for instructions on mapping an external port to the camera’s IP address and port.