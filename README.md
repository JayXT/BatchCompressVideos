# BatchCompressVideos
A simple ffmpeg-based script for compression of all videos in a directory.

A couple of common video formats like mp4, mpg have been taken into consideration, but more could be added. Script compresses videos in the current directory using ffmpeg and saves them into mp4 format. 
Video stream is encoded as HEVC, while audio stream relies on Opus codec.

The algorithm doesn't replace existing files, instead it creates files with the same name, but with added "_compressed" suffix. All already existing files containing "_compressed" substring are skipped.

The script has been tested in Debian 12.
