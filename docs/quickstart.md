### Quickstart

1.
    Download HF Trading Simulator from the following page: [http://tradesim.org/#download]()
    
2.
    Unpack zip archive into local folder and navigate into it
    
3.
    Setup python-3:
      * windows from https://www.python.org/downloads/
      * for debian/ubuntu ``sh sudo apt-get install python3``
      * for centos/fedora ``sh sudo yum install python3``

    There are the following binaries in the archive: ``hfts_get`` and ``hfts_full`` and ``htfs_ohlc``
    * ``htfs_get`` is used to download market data
    * ``htfs_full`` for level3 strategy replay
    * ``htfs_fast`` for level1 or ohlc strategy replay
    * ``htfs_find`` for level1 strategy replay for dynamic parameteres finding.

4.
    Run ```sh hfts_get demo``` to download free demo day

    There are some examples in py_examples folder:

5.
    Run ```sh hfts_play -ohlc py_examples/sma_ohlc.py```

    Report will be generated in JSON format in ``reports`` folder
    
6.
    Run ```sh hfts_play py_examples/simple_hft.py``` for HFT backtesting

    If you have real trade module and want to run it on real exchange, then:
    1. copy ``conf/tsim_example.toml`` into ``conf/tsim.toml`` and then edit it.
    2. ```sh hfts_play -run -ohlc py_examples/simple_sma.py```

* For creating your own strategy, please move to main [documentation](doc.md)

