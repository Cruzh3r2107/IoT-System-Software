# IoT-System-Software

Most of the ESP functionality remains the same. The biggest difference now is at least one of the ESP devices will also have an LED bar graph and show bars based on light intensity level. You will use the circular LED board.
The RPi will be connected to an LED Matrix showing the photocell data trace over the past ~30 seconds, each column representing ~4 seconds.
The RPi will be connected to a 4 digit 7-segment display showing the last 3 digits of the IP address of the current Master.
You will integrate a web server to display pertinent information using Node-RED along w/ IBM's cloud.
RPi is connected with a button. When the button is pressed.
it resets all ESP8266's and turns on its Yellow LED for 3 seconds 
RPi webserver should reset graphs/charts and continue (if doing real-time monitoring).
RPi saves current log file (if any) starts a new logfile with the current date and time as part of the filename.
This logfile should be saved locally to access by the RPi webserver
RPi will display 2 graphs (through the web server) containing the following information.
photocell data trace on its window screen
static option: after a log file is created, the web server should show the graph or let the user select the log file to display.
bar chart showing master devices (identified by IP) and how long they have been master
static option: after a log file is created, the web server should show the chart or let the user select the log file to display.
RPi log file contains current date and time based on button press
log file should contain logged information since the last button press to the current button press of
all devices that became masters (IP addresses)
how long each device was a master (from the beginning) raw data from each master
The system should work with 3-6 ESP8266 devices dynamically (by showing demo starting from powering on one ESP8266, two devices, and then all three devices). RPi should be able to join after the Master of the swarm is shown up. 
