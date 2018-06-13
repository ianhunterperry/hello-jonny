import RPi.GPIO as GPIO
import time

GPIO.setmode(GPIO.BCM)

GPIO.setup(21, GPIO.OUT)
GPIO.setup(13, GPIO.OUT)
GPIO.output(21, GPIO.HIGH)
GPIO.output(13, GPIO.HIGH)

time.sleep(10)

GPIO.output(21, GPIO.LOW)
GPIO.output(13, GPIO.LOW)
GPIO.cleanup()
