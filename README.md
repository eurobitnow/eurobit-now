# Eurobit

# BEFORE USING EUROBIT SIMPLEWALLET/DAEMON OR EUROBIT GUI CLIENT:
## If your daemon is stuck on block 0, or if you do not have any peers, load up the daemon and start it like the following:
> ./eurobitd --add-peer 35.196.218.62:8080

Or

> ./eurobitd --add-peer 35.188.44.219:8080
## Doing this will manually connect you to the seed nodes to allow you to find more peers, if the daemon or GUI client is starting at block 0 exit both and open the daemon with that command, then you may continue to use simplewallet once it is done syncing, or once it is done syncing close the daemon and open up the GUI client and it should start getting blocks as it should normally

## Guide to compiling Eurobit from source on Ubuntu
(If your on Windows just download one of the Windows binarys, no compile needed :D)

## Install depenencies

> sudo apt-get install build-essential git cmake libboost1.55-all-dev

If it wont let you install libboost, then run this command:

> sudo apt-get install libboost-all-dev

## Download the source code

> git clone https://github.com/Codex02/Eurobit

If you don't have git installed, download it through this command:

> sudo apt-get install git

## Get into the directory and compile

> cd Eurobit

> make

This will begin the compile process, which will take a while. Have a cup of tea or something while you wait.

## Go into the build directory

After it's done compiling, you need to go into the folder where the compiled builds are held

> cd build

> cd release

>cd src

## Start the simplewallet/daemon
Now just start the daemon by doing this command:

> ./eurobitd

And after it is done syncing with the blockchain, load the simplewallet with this command

> ./simplewallet

After that your simplewallet and daemon will be fully synced! 

You can also solo mine in the daemon by doing this command: 

> start_mining [your wallet address]
