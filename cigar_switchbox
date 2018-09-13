#sets up the tones for mary had a little lamb, but haven't figured out how to test for a sequence.

from adafruit_circuitplayground.express import cpx
import time
import board

import digitalio

# assign A1 to "switch1"
switch1 = digitalio.DigitalInOut(board.A2)

# assign A2 to "switch2"
switch2 = digitalio.DigitalInOut(board.A3)

# assign A3 to "switch1"
switch3 = digitalio.DigitalInOut(board.A4)

# make switches "pull up", or high voltage when not connected to GND
switch1.pull = digitalio.Pull.UP
switch2.pull = digitalio.Pull.UP
switch3.pull = digitalio.Pull.UP

# wire all pins (A1-A4) to top of case, and ground to bottom of case in correct positions

while True:
    #to prevent false negatives (when contacts don't align perfectly immediately)
    time.sleep(0.5)
    
    #"resting" state - turn off all LEDs and do nothing
    if switch1.value and switch2.value and switch3.value:
        cpx.pixels[0] = ((0, 0, 0))
        cpx.pixels[1] = ((0, 0, 0))
        cpx.pixels[2] = ((0, 0, 0))
        cpx.pixels[3] = ((0, 0, 0))
        cpx.pixels[4] = ((0, 0, 0))
        cpx.pixels[5] = ((0, 0, 0))
        cpx.pixels[6] = ((0, 0, 0))
        cpx.pixels[7] = ((0, 0, 0))
        cpx.pixels[8] = ((0, 0, 0))
        cpx.pixels[9] = ((0, 0, 0))
    
    #success!
    elif not switch1.value and not switch3.value:
        cpx.play_file("Fanfare.wav")
        cpx.pixels[0] = ((0, 3, 0))
        cpx.pixels[1] = ((0, 3, 0))
        cpx.pixels[2] = ((0, 3, 0))
        cpx.pixels[3] = ((0, 3, 0))
        cpx.pixels[4] = ((0, 3, 0))
        cpx.pixels[5] = ((0, 3, 0))
        cpx.pixels[6] = ((0, 3, 0))
        cpx.pixels[7] = ((0, 3, 0))
        cpx.pixels[8] = ((0, 3, 0))
        cpx.pixels[9] = ((0, 3, 0))
        time.sleep(0.1)
        cpx.pixels[0] = ((0, 0, 3))
        cpx.pixels[1] = ((0, 0, 3))
        cpx.pixels[2] = ((0, 0, 3))
        cpx.pixels[3] = ((0, 0, 3))
        cpx.pixels[4] = ((0, 0, 3))
        cpx.pixels[5] = ((0, 0, 3))
        cpx.pixels[6] = ((0, 0, 3))
        cpx.pixels[7] = ((0, 0, 3))
        cpx.pixels[8] = ((0, 0, 3))
        cpx.pixels[9] = ((0, 0, 3))
        time.sleep(0.1)

    else:
        cpx.play_file("Boing.wav")
        cpx.pixels[0] = ((0, 0, 0))
        cpx.pixels[1] = ((0, 0, 0))
        cpx.pixels[2] = ((0, 0, 0))
        cpx.pixels[3] = ((0, 0, 0))
        cpx.pixels[4] = ((0, 0, 0))
        cpx.pixels[5] = ((0, 0, 0))
        cpx.pixels[6] = ((0, 0, 0))
        cpx.pixels[7] = ((0, 0, 0))
        cpx.pixels[8] = ((0, 0, 0))
        cpx.pixels[9] = ((0, 0, 0))
        time.sleep(0.1)
        cpx.pixels[0] = ((3, 0, 0))
        cpx.pixels[1] = ((3, 0, 0))
        cpx.pixels[2] = ((3, 0, 0))
        cpx.pixels[3] = ((3, 0, 0))
        cpx.pixels[4] = ((3, 0, 0))
        cpx.pixels[5] = ((3, 0, 0))
        cpx.pixels[6] = ((3, 0, 0))
        cpx.pixels[7] = ((3, 0, 0))
        cpx.pixels[8] = ((3, 0, 0))
        cpx.pixels[9] = ((3, 0, 0))
        time.sleep(0.1)
