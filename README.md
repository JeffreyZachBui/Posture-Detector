# Posture-Detector
Visualize your posture with graphs, and calibrate your posture to fix it

Users will be able to visualize their back posture with this website.

This works by:

- Arduino with gyroscopes are attached to individual's back
- Realtime data is sent from Arduino to Phant (A service where you can output data online)
- Latest coordinates (from the gyroscope) are constantly being uploaded to the phant
- The website scraps the latest coordinates (json file) from the phant, and updates a line chart (Canvas JS)
- Users have the option of "calibrating their posture." This is for when users sit up straight, then click "calibrate."
  This then returns the latest coordinates and sends it to the next page (via the URL). This is called the posture standard.
  The posture standard is a group of fixed lines on the line chart. Therefore, users can see in real time how far their 
  posture strays from where it should be.
  
 How to use:
 
- Upload the .ino file into the Arduino, then run it. 
- Run website.


This current version just randomly outputs coordinates between -5 and 5, because there have been issues with the gyroscope that this code was originally written for. 
