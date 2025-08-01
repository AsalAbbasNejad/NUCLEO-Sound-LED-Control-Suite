#  NUCLEO Sound & LED Control Suite

This repository contains two embedded systems projects developed for the STM32 NUCLEO platform. The projects demonstrate real-time control of sound playback and LED behavior using GPIO interrupts and timers.

##  Project Contents

### 1. SnapTrigger_LED
- **Function**: Toggles the onboard green LED when a finger snap is detected through a microphone input.
- **Implementation**: Uses an external GPIO interrupt triggered by sound (via SND_IN pin).
- **Learning Outcome**: Handling GPIO interrupts and real-time input detection.

### 2. PlaySong_TimerInterrupt
- **Function**: Plays a melody on the NUCLEO board.
- **Implementation**:
  - Initial version uses `HAL_Delay` to space notes.
  - Enhanced version replaces blocking delays with timer interrupts for non-blocking, efficient control.
- **Learning Outcome**: PWM sound generation, timer configuration, and interrupt-based timing.

---

##  Technologies Used

- **Hardware**: STM32 NUCLEO Development Board
- **Software**: STM32CubeIDE, STM32 HAL Libraries
- **Core Concepts**:
  - GPIO external interrupts
  - Timers and PWM
  - Sound synthesis and timing
  - Non-blocking firmware design

---

## How to Run

1. Clone this repository or download the `.zip` file.
2. Open the projects in **STM32CubeIDE**.
3. Connect your STM32 NUCLEO board via USB.
4. Build and flash the desired project.
5. Interact with the board:
   - Snap near the microphone to toggle the LED.
   - Watch the LED blink or hear the song play.

