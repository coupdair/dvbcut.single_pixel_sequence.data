output of [DVBcut](https://github.com/coupdair/dvbcut) with [Single Pixel Sequence addon](https://github.com/coupdair/dvbcut.src)
, i.e. advertisment cut !

This repository is archiving a few SPS data
, i.e. Single Pixel Sequence along time line
, to find discontinuities that could be advertisment or transition between movie series !

It helps a lot finding where to cut (e.g. start/stop marker within DVBcut software)
, in fact, it does the roughtly the job
, one may ajust by a few frames only.

SPS data is in TIF format, for fast archiving, as it is uncompressed regarding to PNG.
[CImg](https://github.com/coupdair/CImg) library plugin is handling this very fast.

# data example

## pixel within black strip

pixel within black strip of "AntMan" movie from DVB-T stream:
flat lane is the movie, oscillation parts are advertisments.

![pixel within black strip](AntMan_20180429_h6G.mpeg_SPSgraph.png)

## pixel within channel logo

pixel within white of the channel logo for "Underground" movie from DVB-T stream:
flat lane is the movie, oscillating parts are channel streaming advertisments
, i.e. begining and end of the movie.

![pixel within white logo](Underground_20180501.mpeg_SPSgraph.png)
