cd "/Users/edtosoy/Downloads/DreamyReads files/Scripts/"   

Curl -O 

source tts_env/bin/activate 
python google_tts_script.py  
deactivate # when finished   

ffmpeg -i "concat:my_10min_voiceover_01.mp3|my_10min_voiceover_02.mp3|my_10min_voiceover_03.mp3" -acodec copy combined_voiceover.mp3
