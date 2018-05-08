# AudioBug

This app demonstrates the inconsistent audio behaviours among some of Samsung's phones (AT&T models vs others).

The app uses a simple MediaPlayer and AudioRecord instances. The MediaPlayer starts playing music once the app starts. The AudioRecord will start recording once user clicks the "Start recording" button. Please note we use VOICE_COMMUNICATION option in recording to achieve acoustic echo cancellation.

The difference between AT&T phones (S7, S7 Edge) and other carrier models:

* On AT&T phones (we tested on S7, S7 Edge), once the "start recording" button is clicked, the music is **muted (to extremely low volume)**. If the device has other music apps playing in background, they will also get muted. Stop recording will bring the music volume back to normal. 

* On T-Mobile phones, or unlocked versions, or other OEM devices (we tested on MotoX, Kindle Fire and Huawei), the music continues with minor volume damp. 

zhiyun.li@gmail.com
