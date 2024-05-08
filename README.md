![182040678-89dc50d8-6313-47e6-8c23-d0f9eada21fa](https://github.com/mohamedmostaf21/Microwave-oven-controller/assets/87494262/b19d45b0-a707-4335-aad0-a7a299418e36)Microwave-Oven-Controller-Project
This project is for Introduction to Embedded Systems Course. it was written in C using Keil 4.

Aim
simulate the embedded controller in a microwave oven.

Procedure Details:
While not cooking (not at any mode), message is shown on LCD "select a choice"

If A (for popcorn) is pushed on the keypad, the LCD should show "Popcorn" for two seconds and then start cooking for 1 minute while the remaining cook time counts down (in seconds) on the LCD.
If B (for Beef) or C (for chicken) is pushed on the keypad, the LCD should show "Beef weight?" or "Chicken weight?" (respectively) should appear on the LCD until the user enters an integer value between 1 and 9 on the keypad to indicate how many kilos are there to be defrosted. After a valid number is entered, clear the LCD display and show the value of the weight on the LCD for two seconds, and then start cooking while the remaining cook time counts down (in seconds) on the LCD. o Beef is defrosted at a rate of 0.5 minutes per kilo. o Chicken is defrosted at a rate of 0.2 minutes per kilo. o If an illegal number is entered, the LCD should show "Err" for two seconds, then show previous message.
If D (for entering certain time) is pushed on the keypad, the LCD should show "Cooking time?" until the user enters a value between 1 and 30 to indicate the cooking time required in minutes and seconds. o This value is displayed on the LCD as it is entered as the following example pressing 1 displays 00:01, then pressing 2 displays 00:12, then pressing 4 displays 01:24, then pressing 5 displays 12:45
Start/Stop/Pause cooking conditions:
Switch SW3 (external push button) will simulate the microwave oven door latch, where the switch being down would be simulating the open-door situation and the switch being up would be simulating the door closed situation.
Only when the latch is closed should the oven be able to be started.
When SW1 is pressed for first time, the oven operation pauses (keeping remaining time on the display).
When SW1 is pushed for second time after pressing it for first time, the time is cleared and the cooking stops.
If SW2 is pushed after the oven is paused and the door is closed, then cooking must resume from the time it was paused.
If it is cooking, opening the door should pause the cooking and keep the remaining time on display.
When the microwave is running, the array of LEDs should be on.
When it is stopped (no choice is entered), the array of LEDs should go off.
When the microwave is paused, the array of LEDs should blink (wait till the cooking is resumed or stopped).
When the microwave completes its function (timer has counted down to zero), the array of LEDs should flash 3 times then the buzzer should be on for 3s.
Processes Diagram
image
![182040678-89dc50d8-6313-47e6-8c23-d0f9eada21fa](https://github.com/mohamedmostaf21/Microwave-oven-controller/assets/87494262/245cd3c1-c95c-4af2-9911-f5eb2f1699dc)
