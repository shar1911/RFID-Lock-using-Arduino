# RFID-Lock-using-Arduino
Features
1)RFID Reader: Utilizes an MFRC522 RFID reader to scan RFID tags.\n
LCD Display: Provides real-time feedback to the user through a 16x2 LiquidCrystal I2C LCD screen.
LED Indicators: Green and red LEDs indicate access granted or denied.
Relay Control: Manages an electromagnetic lock or other actuators via a relay.
Buzzer Alerts: Provides audio feedback for access denial.
Components
Arduino Uno: The microcontroller board that coordinates all activities.
MFRC522 RFID Reader: Reads RFID tags for identification.
LiquidCrystal I2C LCD (16x2): Displays messages to the user.
LEDs (Green and Red): Indicate access status.
Relay Module: Controls the locking mechanism.
Buzzer: Alerts when access is denied.
How It Works
Initialization: The system initializes the RFID reader, LCD, LEDs, relay, and buzzer.
Card Detection: The system continuously scans for RFID tags.
UID Reading: When a tag is detected, the system reads its unique identifier (UID).
Access Decision: The system compares the UID with a list of authorized IDs.
Authorized Access: If the UID matches, the relay activates to unlock the door, the green LED lights up, and the LCD displays "Access Granted."
Access Denied: If the UID does not match, the red LED lights up, the buzzer sounds, and the LCD displays "Access Denied."
Reset: After a short delay, the system resets and is ready for the next card scan.
Applications
Office Security: Restricts access to sensitive areas in an office environment.
Laboratories: Manages entry to research labs requiring high security.
Residential: Controls access to private homes or apartment buildings.
Industrial: Secures entry points in industrial facilities.
Code Explanation
The provided Arduino code initializes the system components, reads RFID tags, and checks the UID against pre-defined authorized IDs. Depending on the result, it grants or denies access, providing visual and audio feedback accordingly.


