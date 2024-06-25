# RFID-Lock-using-Arduino
Features
1)RFID Reader: Utilizes an MFRC522 RFID reader to scan RFID tagss
2)LCD Display: Provides real-time feedback to the user through a 16x2 LiquidCrystal I2C LCD screen.
3)LED Indicators: Green and red LEDs indicate access granted or denied.
4)Relay Control: Manages an electromagnetic lock or other actuators via a relay.
5)Buzzer Alerts: Provides audio feedback for access denial.
Components
1)Arduino Uno: The microcontroller board that coordinates all activities.
2)MFRC522 RFID Reader: Reads RFID tags for identification.
3)LiquidCrystal I2C LCD (16x2): Displays messages to the user.
4)LEDs (Green and Red): Indicate access status.
5)Relay Module: Controls the locking mechanism.
6)Buzzer: Alerts when access is denied.
How It Works
1)Initialization: The system initializes the RFID reader, LCD, LEDs, relay, and buzzer.
2)Card Detection: The system continuously scans for RFID tags.
3)UID Reading: When a tag is detected, the system reads its unique identifier (UID).
4)Access Decision: The system compares the UID with a list of authorized IDs.
5)Authorized Access: If the UID matches, the relay activates to unlock the door, the green LED lights up, and the LCD displays "Access Granted."
6)Access Denied: If the UID does not match, the red LED lights up, the buzzer sounds, and the LCD displays "Access Denied."
7)Reset: After a short delay, the system resets and is ready for the next card scan.
Applications
1)Office Security: Restricts access to sensitive areas in an office environment.
2)Laboratories: Manages entry to research labs requiring high security.
3)Residential: Controls access to private homes or apartment buildings.
4)Industrial: Secures entry points in industrial facilities.



