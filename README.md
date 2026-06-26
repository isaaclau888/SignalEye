# SignalEye
<img width="1920" height="1080" alt="SignalEye_2026-Jun-18_06-48-48AM-000_CustomizedView6057489903_png" src="https://github.com/user-attachments/assets/ee77af41-579e-4660-9235-ea6afca9f135" />

Imagine living in a flat with a security guard downstairs, but a thief can still come to your flat, steal your stuff and run away (This is not my situation, just an imagination only; it's fake). To prevent this kind of thing from happening, you MUST have SignalEye, your home guardian; it lets you check who is outside your door.    

## What's it for?
It's for home safety. It prevents burglary from happening. With a Smart Doorbell, you can know who comes to your home.

## How to build it?
Please print all the 3D parts. <p>
<img width="688" height="456" alt="螢幕截圖 2026-06-18 下午4 03 06" src="https://github.com/user-attachments/assets/15ec6709-e8b2-45f1-a6db-f11f7b543bc5" />


# 3D Parts Assembly
First, place the bottom part. <p>
<img width="686" height="479" alt="螢幕截圖 2026-06-18 下午4 04 05" src="https://github.com/user-attachments/assets/7fc80f57-ff1e-46df-87d6-0cceabcb5e07" />


Secondly, place the ESP32-CAM with the camera, ESP32-CAM-MB, which connects the cable to the 18650 lithium battery expansion board with one 18650 lithium battery inside the bottom case. <p>
<img width="650" height="485" alt="螢幕截圖 2026-06-18 下午4 06 01" src="https://github.com/user-attachments/assets/d7c329ee-81f4-45e2-949d-6512f2f2e46b" />

Thirdly, connect the connectors. <p>
<img width="685" height="492" alt="螢幕截圖 2026-06-18 下午4 14 36" src="https://github.com/user-attachments/assets/d9e4f2e0-ba13-49f6-9f14-c18860b56900" />


Last but not least, place the top part on top. <p>
<img width="595" height="490" alt="螢幕截圖 2026-06-18 下午4 15 33" src="https://github.com/user-attachments/assets/59b64ae4-e2c1-4740-885c-0aadeeb0c421" />

# Wiring Diagram
<img width="5000" height="4362" alt="SignalEye Wiring Diagram" src="https://github.com/user-attachments/assets/346a5919-8669-4811-9ba6-0cd08a33696c" />

Just follow the diagram. <p>
Use a green jumper wire to connect IO12 on the Burner Base -> Connects to Green (NO) on the button <p>
Use a green jumper wire to connect GND on the Burner Base -> Connects to the other Green (NO) on the button <p>
Use a red jumper wire to connect 3V3 on the Burner Base -> Connects to Red (+) on the button <p>
Use a black jumper wire to connect GND on the Burner Base -> Connects to Black (-) on the button <p>
And for the power supply, connect the USB-C part of the wire to the ESP32-CAM-MB, connect the USB-A part of the wire to the 18650 lithium battery expansion board, which has one 18650 lithium battery inside. <p>
If you need another 18650 lithium battery, you must charge it with a charger and connect it like that. <p>

## How can you use it?
1. Install Arduino IDE:
Download and install the latest Arduino IDE from the official Arduino website.
2. Install ESP32 Board Core:
Open Arduino IDE and go to File > Preferences. 
In the Additional Boards Manager URLs field, paste this URL: 
https://espressif.github.io/arduino-esp32/package_esp32_index.json 
Click OK.
Go to Tools > Board > Boards Manager, search for ESP32, and click Install.
3. Select Your Board and Port:
Go to Tools > Board > ESP32 and select AI Thinker ESP32-CAM.
Plug your black burner programming base into your computer via a USB cable.
Go to Tools > Port and select the correct port for your connected board.
4. Upload the Code:
Load your complete SignalEye.ino code into the workspace.
Update the Wi-Fi SSID, password, and your personal Slack webhook path lines inside the script.
Click the Upload arrow button in the top-left corner. After a few seconds, it will finish uploading!
5. Fire It Up:
Open your Serial Monitor (Tools > Serial Monitor), set the speed to 115200 baud, and press the physical Reset button on your board. Watch your smart doorbell connect to the network and trigger your first Slack alert! Yay!!!

## Why did I make it?
I decided to make this because I want to keep my home safe; I don't want random people knocking on my door.

## How I made it?
I used Fusion 360 to make the snap-fit case, Arduino IDE for the coding part and last but not least, the parts from the BOM.

# Fallout Zine 
<img width="4405" height="6250" alt="SignalEye Fallout Zine" src="https://github.com/user-attachments/assets/80f2ab37-8cd0-4bc9-942c-08b5bf5e2c7b" />
