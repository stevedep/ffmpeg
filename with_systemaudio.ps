#deze werkt met webcam, scaling, image overlay and system audio, press F6 for volume, boost is hier maar 6, dan zitten ze ons op één lijn!!
C:\Temp\bin\ffmpeg ` -y -rtbufsize 900M <# Big Buffer Size for Webcam stream #>`
-f dshow -i video="Integrated Camera":audio="Headset Microphone (2- Plantronics Blackwire 315.1)" <# Input 0 with audio and video #> `
-f gdigrab -offset_x -268 -offset_y -1440 -video_size 2560x1400 -i desktop <# Input 1 #> `
-i "C:\Temp\Banner_Visual_Development.png" <# Input 2 #>`
-f dshow -i audio="CABLE Output (VB-Audio Virtual Cable)" <# Input 3 #>` `
-c:v libx264 -r 20 -preset ultrafast -tune zerolatency -crf 0 -pix_fmt yuv420p `
-filter_complex ("`
[0:a]volume=volume=6[a];" + <# Aplifiy Volume #> `
"[0:v]scale=300:trunc(ow/a/2)*2[s];" + <# Scale Webcam #>`
"[1:v][s]overlay=(main_w-overlay_w):main_h-overlay_h[v];" + <# Overlay Webcam on video #>`
"[v][2]overlay=(main_w-overlay_w):0[v2];" + <# Overlay Banner #>`
"[a][3]amix[mix]" + <# Mix System sound with mic #>`
"") -map "[v2]" -map "[mix]" "C:\Temp\-$(get-date -f yyyy-MM-dd-Hmss).mkv"   
