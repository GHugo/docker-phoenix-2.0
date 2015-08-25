## Phoenix-2.0

Container for phoenix-2.0 (see [official repository](https://github.com/kozyraki/phoenix/)).
Automatically download datasets.

### Installation
Retrieve the image from DockerHub:

`docker pull ghugo/phoenix-2.0`


### Usage

Launch word_count on the 100MB dataset:

`docker run ghugo/phoenix-2.0 /phoenix/phoenix-2.0/tests/word_count/word_count /data/word_count_datafiles/word_100MB.txt`

Time histogram execution:

`docker run ghugo/phoenix-2.0 bash -c "time /phoenix/phoenix-2.0/tests/histogram/histogram /data/histogram_datafiles/small.bmp"`

All the datasets are in **/data**.

The phoenix sample applications are in **/phoenix/phoenix-2.0/tests**.