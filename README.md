# stitch
Stitch together media files with a given file extension in the current working directory. Relies on (and is effectively just a pretty abstraction over) [ffmpeg](https://www.ffmpeg.org).

Install by adding the `stitch` script file to your `PATH`, and make sure it's marked as executable.

Usage: `stitch <file extension> <output file>`

## Example
Imagine your current working directory contains these files:
* `1.mp3`
* `2.mp3`
* `5.m4a`
* `10.m4a`

Running `stitch mp3 out.mp3` would create a new file, `out.mp3`, which would be the files `1.mp3` and `2.mp3` played one after the other.

## Why?
Imagine a radio station, recording all its output 24/7, each hour into its own file. What if you wanted to stitch a few of those audio files together into one, so you could listen to a whole show as it was originally broadcast? This script makes that easier and saves opening up a full editing tool. It's also faster than any editing tool I've seen.
