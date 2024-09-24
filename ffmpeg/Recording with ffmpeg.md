Use the following command to find all the audio recording devices you have avaliable
arecord -l

To start recording audio
ffmpeg -f alsa -i hw:0,0 output_audio.wav

where hw:card 0, device 0
