# Gloves for Deaf and dump - Project

## Overview

This project involves a pair of smart gloves designed to assist individuals who are deaf and dump by converting hand gestures into voice messages. The system uses various components to detect hand gestures and provide audio feedback through a speaker. The project utilizes an ADC to read analog values from sensors, an LCD to display messages, and a DFPlayer module for audio playback.

## Components Used

- **Microcontroller**: (Specify your microcontroller, e.g., ATmega328P)
- **ADC (Analog-to-Digital Converter)**: To convert analog signals to digital.
- **LCD**: To display messages.
- **DFPlayer Mini**: For playing audio tracks.
  ![dfplayer](https://github.com/user-attachments/assets/50498545-3408-4ec4-b702-2a50e038f6e0)
- **8 Ohm 0.5 Watt speaker**
  ![speaker](https://github.com/user-attachments/assets/6b6095f7-e67e-4262-b7a1-3ea92339a4b3)
- **USART (Universal Synchronous and Asynchronous serial Receiver and Transmitter)**: For serial communication.
- **Sensors**: ( flex sensors )
  ![flex](https://github.com/user-attachments/assets/2d197797-e372-4ebd-bd27-e326f0f7c453)

  

## Project Description

The gloves are equipped with sensors that detect hand gestures and provide corresponding voice messages. The system works as follows:

1. **Initialization**: 
   - The LCD and ADC are initialized.
   - The USART communication is set up for interacting with the DFPlayer Mini.

2. **Gesture Detection**:
   - The sensors send analog signals that are read by the ADC.
   - Based on the value read, a specific action is performed:
     - **Low Value (<=250)**: Display "Hello" and play a corresponding audio track.
     - **Medium Value (251-500)**: Display "my name is..." and play a different audio track.
     - **High Value (>500)**: Display "bye" and play a farewell audio track.

3. **Audio Feedback**:
   - The DFPlayer Mini plays pre-recorded audio tracks based on the detected gesture.

## Usage

1. **Power On**: Ensure the system is powered on and the sensors are properly positioned on the gloves.
2. **Gesture**: Perform a hand gesture.
3. **Observe**: The LCD will display a message, and the DFPlayer Mini will play the corresponding audio track.




