## Phoenix-2.0

Container for phoenix-2.0 (see [official repository](https://github.com/kozyraki/phoenix/)).
It also contains the data-sets.

[This article](http://hugoguiroux.blogspot.fr/2015/08/docker-experiment-packaging-pheonix-20.html) explains how and why I decided to build this container.

### Installation
Retrieve the image from DockerHub:

`docker pull ghugo/phoenix-2.0`


### Usage

Launch word_count on the 100MB data-set:

`docker run ghugo/phoenix-2.0 /phoenix/phoenix-2.0/tests/word_count/word_count /data/word_count_datafiles/word_100MB.txt`

Time histogram execution:

`docker run ghugo/phoenix-2.0 bash -c "time /phoenix/phoenix-2.0/tests/histogram/histogram /data/histogram_datafiles/small.bmp"`

All the data-sets are in **/data**.

The phoenix sample applications are in **/phoenix/phoenix-2.0/tests**.