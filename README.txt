This is a patched version of tablet-encode
(http://mediautils.garage.maemo.org/tablet-encode.html) with support
for embedding subtitles as it encodes the video.

I sent this as a patch to Andrew Flegg, with the following description,
but it has so far not been included.

"I tried to use the --mencoder option, but it never worked out for me,
possibly because the -sub option in mencoder needs an argument and
it was not handled well. In addition it took me a fair bit of time to
research how to add subtitles, what formats were accepted and so on. I
think this small patch is a useful addition to tablet-encode that will
save people effort.

It takes as argument a subtitle file and hands it to the -sub option
for mencoder. This can be a file in the srt format and possible others
but not vobsub.  Seems mencoder does not support embedding vobsub.
mencoder by default will use the font specified in ~/.mplayer/subfont.ttf"
