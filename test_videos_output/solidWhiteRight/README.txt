ffmpeg -i solidWhiteRight.mp4 -r 1 -vf scale=-1:120 -vcodec png capture-%002d.png
montage -title "solidWhiteRight" -tile 4x -geometry +4+4 capture*.png output.png