# MEncoder
A 3d to 3d video converting tool for linux by MPlayer. 


# Usage:

to convert SBS 3d video into Anaglyph Red-Cyan/Blue video:

let's assume that we have a file named sbs.mp4 and we want to make anaglyph format of that video at the location of anaglyph.mp4

    ./mencoder -vf stereo3d,scale sbs.mp4 -o anaglyph.mp4 -oac pcm -ovc x264

to specify Aspect ratio:

    ./mencoder -vf stereo3d,scale sbs.mp4 -o anaglyph.mp4 -oac pcm -force-avi-aspect 16:9 -ovc x264
