# 6miner

6miner is a highly optimized cryptocurrency miner that runs on modern AMD / NVIDIA GPUs and CPU. 
* 6miner currently supports [handshake](https://handshake.org/)(blake2b + sha3) algorithm with 3% of devfee.

## Quick start
* Download and extract 6miner into a folder.
* Depending on the coins that you want to mine, find the corresponding script in the folder.(e.g `mine_hns.sh`).
* Change the address and vendor information in the script.
* Run the script and Enjoy mining.

## Reference performances
| algorithm | card | hashrate | 
| --- | --- | --- |
| handshake(blake2b + sha3) | 2080Ti | 340MH/s |
| handshake(blake2b + sha3) | 2060 | 155MH/s |
| handshake(blake2b + sha3) | RX 580 | 64MH/s |
| handshake(blake2b + sha3) | P100 | 84MH/s |


## Command line options
```
  -a, --algo=ALGO          specify the algorithm to use
                             hns/bl2bsha3
  -o, --url=URL             URL of mining server
  -O, --userpass=U:P        username:password pair for mining server
  -u, --user=USERNAME       username for mining server
  -p, --pass=PASSWORD       password for mining server
  -m, --mode=MODE           options: CPU\CUDA\OPENCL (default: CPU)
      --devices=N           list of GPU devices to use.
      --temperature-limit=N limit maximun temperature of GPU
      --opcl-vendor=VENDOR  vendor name, default AMD (options: AMD NVIDIA Intel).
      --no-color            disable colored output
  -B, --background          run the miner in the background
      --print-time=N        print hashrate report every N seconds
      --dry-run             test configuration and exit
  -h, --help                display this help and exit
  -V, --version             output version information and exit
```
