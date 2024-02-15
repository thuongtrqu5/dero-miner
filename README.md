# AstroBWTv3 Dero Miner by DeroLuna

A new optimized AstroBWTv3 Dero CPU Miner.\
As testing shows, it works 4-5 times faster for AMD Ryzen processors and 2-4 times faster for Intel processors than the official miner.

Available for Linux, Windows and HiveOS.

If you have problems with the miner, message me in Discord.\
Discord server: https://discord.gg/vuJW8UahRV

Developer fee: 10%

## Usage ##

```
deroluna-miner -d <daemon-address:port> -w <wallet_address> [-t <threads>]
```

#### Example (Linux)
```
./deroluna-miner -d minernode1.dero.io:10100 -w dero1qykyta6ntpd27nl0yq4xtzaf4ls6p5e9pqu0k2x4x3pqq5xavjsdxqgny8270
```
#### Example (Windows)
```
deroluna-miner.exe -d minernode1.dero.io:10100 -w dero1qykyta6ntpd27nl0yq4xtzaf4ls6p5e9pqu0k2x4x3pqq5xavjsdxqgny8270
```

### Options ###
```
    --help -h
        Shows help
    --version
        Shows the version

    --daemon-address -d
        The daemon address
    --wallet -w
        Your wallet address
    --threads -t
        Number of threads
    --no-lock
        Disables CPU core binding
    --period <time in seconds>
        The period for which the average hashrate is calculated (10 by default)
        Must be between 1 and 64
    --log-console-line <time in seconds>
        Enables logging of the console line with the specified period
    --show-pool-shares
        Shows the total count of shares sent to the pool
    --never-stop
        Simulate mining when connection is lost

    --exit-on-zero-hashrate
        Stops the miner if the hashrate has been zero for 15 seconds
        You should run the command in a loop for the miner to restart (except for HiveOS)
          See the examples in start.sh and start.bat

    --old-console
        Changes the way text is output to the console
    --no-colors
        Removes colors from the console
    --no-cr
        Replaces the carriage return (\r) with a new line (\n) in the console

    --debug-shares
        Shows info about found shares (the JSON message and the hash)
    --debug-getwork
        Shows info about getwork (the JSON message)

    --algo2 0
        Disables optimisations from Beta 1.11.2a
```

## Quick installation ##
#### Linux ####
```
curl -Lo deroluna-miner-linux-amd64.tar.gz https://github.com/DeroLuna/dero-miner/releases/latest/download/deroluna-miner-linux-amd64.tar.gz
tar -xf deroluna-miner-linux-amd64.tar.gz
```

## Hashrate stats ##

#### The maximum average observed hashrate

<details>
  <summary>AMD</summary>

```
AMD Athlon 3000G        4.3 kh/s

AMD Ryzen 3 1200        5.5 kh/s
AMD Ryzen 3 2200G       5.6 kh/s
AMD Ryzen 3 3200G       6.1 kh/s
AMD Ryzen 3 4100        8.7 kh/s
AMD Ryzen 3 4300GE      7.8 kh/s
AMD Ryzen 3 5300U       7.7 kh/s

AMD Ryzen 5 1400        7.6 kh/s
AMD Ryzen 5 1500X       8.2 kh/s
AMD Ryzen 5 1600       13.1 kh/s
AMD Ryzen 5 2400G       7.7 kh/s
AMD Ryzen 5 2500U       6.3 kh/s
AMD Ryzen 5 2600       13.6 kh/s
AMD Ryzen 5 2600X      14.4 kh/s
AMD Ryzen 5 PRO 3400GE  7.2 kh/s
AMD Ryzen 5 3400G       8.6 kh/s
AMD Ryzen 5 3500U       6.0 kh/s
AMD Ryzen 5 3500X      10.5 kh/s
AMD Ryzen 5 3550H       5.5 kh/s
AMD Ryzen 5 3600       16.3 kh/s
AMD Ryzen 5 3600X      16.3 kh/s
AMD Ryzen 5 3600XT     15.4 kh/s
AMD Ryzen 5 4500       15.0 kh/s
AMD Ryzen 5 4600G      15.8 kh/s
AMD Ryzen 5 4600H      11.3 kh/s
AMD Ryzen 5 PRO 4650G  14.6 kh/s
AMD Ryzen 5 5500       18.0 kh/s
AMD Ryzen 5 5500U      12.2 kh/s
AMD Ryzen 5 5600       18.5 kh/s
AMD Ryzen 5 5600G      17.9 kh/s
AMD Ryzen 5 5600H      13.2 kh/s
AMD Ryzen 5 5600X      18.7 kh/s
AMD Ryzen 5 7500F      22.7 kh/s
AMD Ryzen 5 7600       20.6 kh/s
AMD Ryzen 5 7600X      19.7 kh/s

AMD Ryzen 7 1700       17.1 kh/s
AMD Ryzen 7 1700X      16.3 kh/s
AMD Ryzen 7 1800X      17.0 kh/s
AMD Ryzen 7 2700       16.8 kh/s
AMD Ryzen 7 2700X      19.1 kh/s
AMD Ryzen 7 3700X      21.4 kh/s
AMD Ryzen 7 3800X      21.7 kh/s
AMD Ryzen 7 3800XT     17.7 kh/s
AMD Ryzen 7 4700U       8.0 kh/s
AMD Ryzen 7 PRO 4750U  10.6 kh/s
AMD Ryzen 7 4800H      15.9 kh/s
AMD Ryzen 7 4800U      11.3 kh/s
AMD Ryzen 7 5700G      25.4 kh/s
AMD Ryzen 7 5700U      13.1 kh/s
AMD Ryzen 7 5700X      25.5 kh/s
AMD Ryzen 7 5800H      17.0 kh/s
AMD Ryzen 7 5800X      25.3 kh/s
AMD Ryzen 7 5800X3D    23.0 kh/s
AMD Ryzen 7 6800H      18.4 kh/s
AMD Ryzen 7 7700       28.4 kh/s
AMD Ryzen 7 7700X      29.2 kh/s
AMD Ryzen 7 7730U      11.9 kh/s
AMD Ryzen 7 7735HS     19.5 kh/s
AMD Ryzen 7 7800X3D    23.8 kh/s

AMD Ryzen 9 3900       32.2 kh/s
AMD Ryzen 9 3900X      33.1 kh/s
AMD Ryzen 9 3900XT     31.1 kh/s
AMD Ryzen 9 3950X      41.6 kh/s
AMD Ryzen 9 5900HX     17.5 kh/s
AMD Ryzen 9 5900X      37.5 kh/s
AMD Ryzen 9 5950X      47.9 kh/s
AMD Ryzen 9 6900HX     19.7 kh/s
AMD Ryzen 9 7900       43.4 kh/s
AMD Ryzen 9 7900X      43.0 kh/s
AMD Ryzen 9 7900X3D    38.9 kh/s
AMD Ryzen 9 7940HS     20.9 kh/s
AMD Ryzen 9 PRO 7945   35.7 kh/s
AMD Ryzen 9 7950X      57.1 kh/s
AMD Ryzen 9 7950X3D    53.6 kh/s

AMD Ryzen Threadripper 1920X     26.0 kh/s
AMD Ryzen Threadripper 1950X     31.8 kh/s
AMD Ryzen Threadripper 2950X     32.0 kh/s
AMD Ryzen Threadripper 2970WX    39.9 kh/s
AMD Ryzen Threadripper 2990WX    28.6 kh/s
AMD Ryzen Threadripper 3970X     73.4 kh/s
AMD Ryzen Threadripper 3990X    145.2 kh/s
AMD Ryzen Threadripper 7970X     89.8 kh/s
```
</details>

<details>
  <summary>Intel</summary>

```
Intel Core i3-8100       3.3 kh/s
Intel Core i3-9100       3.5 kh/s
Intel Core i3-9100F      3.7 kh/s
Intel Core i3-10100      4.3 kh/s
Intel Core i3-10100F     4.4 kh/s
Intel Core i3-10105      4.5 kh/s
Intel Core i3-1115G4     3.9 kh/s

Intel Core i5-4690K      3.1 kh/s
Intel Core i5-6500       3.0 kh/s
Intel Core i5-6600       3.1 kh/s
Intel Core i5-6600K      3.2 kh/s
Intel Core i5-7400       3.0 kh/s
Intel Core i5-7500       3.3 kh/s
Intel Core i5-7600K      3.7 kh/s
Intel Core i5-8400       4.9 kh/s
Intel Core i5-8500       5.2 kh/s
Intel Core i5-8500T      4.1 kh/s
Intel Core i5-8600       4.3 kh/s
Intel Core i5-8600K      5.0 kh/s
Intel Core i5-9400       5.4 kh/s
Intel Core i5-9400F      5.4 kh/s
Intel Core i5-9500       5.6 kh/s
Intel Core i5-9500T      3.3 kh/s
Intel Core i5-9600K      6.1 kh/s
Intel Core i5-10300H     4.1 kh/s
Intel Core i5-10400      6.2 kh/s
Intel Core i5-10400F     6.6 kh/s
Intel Core i5-10500      6.3 kh/s
Intel Core i5-10600      6.5 kh/s
Intel Core i5-10600K     6.7 kh/s
Intel Core i5-1135G7     6.1 kh/s
Intel Core i5-11400     12.9 kh/s
Intel Core i5-11400F    12.6 kh/s
Intel Core i5-11400H     9.7 kh/s
Intel Core i5-11600K    11.3 kh/s
Intel Core i5-12400F    13.7 kh/s
Intel Core i5-12500     12.8 kh/s
Intel Core i5-12500T     9.4 kh/s
Intel Core i5-13400     18.5 kh/s

Intel Core i7-3770       3.1 kh/s
Intel Core i7-3770K      3.7 kh/s
Intel Core i7-4770K      3.8 kh/s
Intel Core i7-4790       3.7 kh/s
Intel Core i7-4790K      4.0 kh/s
Intel Core i7-5820K      5.0 kh/s
Intel Core i7-6700       3.8 kh/s
Intel Core i7-6700HQ     3.1 kh/s
Intel Core i7-6700K      3.7 kh/s
Intel Core i7-6850K      5.4 kh/s
Intel Core i7-7700       4.1 kh/s
Intel Core i7-7700K      4.7 kh/s
Intel Core i7-8700       6.3 kh/s
Intel Core i7-8700K      6.9 kh/s
Intel Core i7-8750H      4.6 kh/s
Intel Core i7-9700       8.2 kh/s
Intel Core i7-9750H      4.3 kh/s
Intel Core i7-10510U     3.2 kh/s
Intel Core i7-1065G7     4.5 kh/s
Intel Core i7-10700      9.5 kh/s
Intel Core i7-10700F     7.6 kh/s
Intel Core i7-10700K     9.6 kh/s
Intel Core i7-10700KF    8.0 kh/s
Intel Core i7-11700     10.9 kh/s
Intel Core i7-11700F    15.9 kh/s
Intel Core i7-11800H    11.7 kh/s
Intel Core i7-12650H     8.5 kh/s
Intel Core i7-12700     19.2 kh/s
Intel Core i7-12700H    15.7 kh/s
Intel Core i7-13700F    12.1 kh/s
Intel Core i7-13700HX   21.8 kh/s
Intel Core i7-13700K    32.8 kh/s

Intel Core i9-7940X     11.1 kh/s
Intel Core i9-9900K      9.9 kh/s
Intel Core i9-9900KF     8.2 kh/s
Intel Core i9-10850K    12.6 kh/s
Intel Core i9-10980XE   19.7 kh/s
Intel Core i9-11900H    11.5 kh/s
Intel Core i9-11900KF   15.8 kh/s
Intel Core i9-14900KF   45.3 kh/s
```
</details>

## Known issues
* May crash on Linux when resolving the daemon address with the "Assertion failed" exception. In this case, just run the program again.
* If you have a dual CPU and you are using Windows, then most likely only one of the CPUs will be used. To use the second CPU, run another instance of the miner.
