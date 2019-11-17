### Quickstart

1. Dowwnload HF Trading Simulator from the following page: [http://tradesim.org/#download]()
2. Unpack zip archive into local folder and navigate into it
3. Setup python-3:
* windows from https://www.python.org/downloads/
* for debian/ubuntu sudo apt-get install python3
* for centos/fedora sudo yum install python3

There are binaries in the archive: tsim_get and tsim_play
run ```sh hfts_get demo``` to download free demo day

There are some examples in py_examples folder
Run ```sh hfts_play -ohlc py_examples/sma_ohlc.py```
Report will be generated in JSON format in reports folder
Run ```sh hfts_play py_examples/simple_hft.py``` for hft backtesting
If you have real trade module and want to run it on real exchange, then:
copy conf/tsim_example.toml into conf/tsim.toml and then edit
```sh hfts_play -run -ohlc py_examples/simple_sma.py```
For creating your own strategy, please move the next slide slide