# ffmpeg-to-webrtc

Demonstration of screen capture [pion](https://github.com/pion/webrtc).

## How to run it

### Open example web page
[codepen.io](https://codepen.io/ppjln/pen/oEZXjV)
Copy test.html text into codepen.
Wait for it to generate SDP

### Copy browser's SDP
In the codepen.io the top textarea is your browser's SDP, copy that to clipboard.

### Paste it into file
Put copied SDP into SDP.txt file

### Before run
Make sure to have ffmpeg installed:
run:

"$ sudo apt install ffmpeg"

### Copy+Paste cmd from testcapture
From the testacpture file copy command and edit it.
*-video_size []x[] - setup monitor capture zone
*-video_size []    - setup framerate
*-i :0.0 +[]       - setup monitor number (with one display keep as it is) + offset(offset<=mon1+mon2+..+monk)

Run it from src folder!

### Put SDP from ffmpeg-to-webrtc into your browser
When you see SDP in base64 format printed it means that SDP is already in clipboard. 

So you can go to codepen.io page and paste that into Application SDP text area.

### Hit 'Start Session' in codepen
A video should start playing in your browser below the input boxes.

Delay must get lower in a few seconds


### Sound folder
Undone feature. 

