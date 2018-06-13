import RPi.GPIO as GPIO
import time

GPIO.setmode(GPIO.BCM)

GPIO.setup(21, GPIO.OUT)
GPIO.setup(26, GPIO.OUT)
GPIO.output(21, GPIO.HIGH)
GPIO.output(26, GPIO.HIGH)

time.sleep(5)

GPIO.output(21, GPIO.LOW)
GPIO.output(26, GPIO.LOW)
GPIO.cleanup()
