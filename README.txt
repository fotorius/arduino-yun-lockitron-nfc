Author:   Alfredo Rius
License:  BSD(LICENSE)

    This is an implementation of the NFC breakout for the PN532 from Adafruit
    and the Lockitron platform to allow access to doors. With web app. This
    project is related to a previous project arduino-yun-lockitron located in
    https://github.com/devalfrz/arduino-yun-lockitron where you can find the
    configuration of the web server under the www directory.

    This program is based on the arduino-lockitron-nfc shield located (Eagle
    files in https://github.com/devalfrz/arduino-lockitron-nfc).

    Buttons: (buttons are set to have a pullup resistor so they ar inverted)
      - SLOT_SELECT: Selects a memory slot. STATUS_LED will blink n times depending
          on the slot that has been selected.
            
      - MEMORY_BUTTON: If it's pressed for 3 seconds while a card is read,
          it will either override the selected slot or delete the card if it
          was already registered.

      - LOCK_UNLOCK: This button will lock or unlock the system depending on its
          previous state.
          
