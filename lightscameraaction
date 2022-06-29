<pre class="wp-block-syntaxhighlighter-code">#Import Camera, time and GPIO libraries
from picamera import PiCamera
from time import sleep
import RPi.GPIO as GPIO
#We will be using GPIO output pin 18. This pin is connected to the LED light.
GPIO.setmode(GPIO.BCM)
GPIO.setup(18, GPIO.OUT)
#naming our PiCamera 'camera'
camera=PiCamera()
#Starting by turning off our output pin 18
GPIO.output(18, False)
#Setting resolution of our camera
camera.resolution=(2592, 1994)
camera.framerate=15
#Turning our camera on
caemra.start_preview()
#Adding text to the photo
camera.annotate_text="test photo"
camera.annotate_text_size=100
#Letting the camera be in preview mode for 5 seconds
sleep(5)
#Snap the photo, save it to desktop and turn the camera off, ie stop the preview
camera.capture('/home/pi/Desktop/image.jpg)
camera.stop.preview ()
#Activate the light bulb, connected to GPIO pin 18
GPIO.output(18, true)
</pre>
