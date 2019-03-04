# OLED-128x64-I2C-configration-with-moOde
Brief description to setup Moode Audio with Oled display 128x64 

STEPS

sudo apt-get update

sudo raspi-config

sudo apt-get install build-essential python-pip python-dev python-smbus git python-imaging python-mpd

sudo apt-get install -y python-dev python3-dev

sudo apt-get install -y python-imaging python-smbus i2c-tools

i2cdetect -y 1


git clone https://github.com/adafruit/Adafruit_Python_GPIO.git 

cd Adafruit_Python_GPIO 

sudo python setup.py install 

cd ..

git clone https://github.com/adafruit/Adafruit_Python_SSD1306.git 

cd Adafruit_Python_SSD1306

sudo python setup.py install

cd ..

git clone https://github.com/naisema/MoodeAudio-OLED.git

menu -> Configure -> System -> Local Services -> LCD update engine fille full path of python script. On button and apply SET 

/home/pi/MoodeAudio-OLED/moode-oled.py
