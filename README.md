# GUI for EWBF miner
GUI for EWBF miner for monitoring (cool graphs) performance with restart capability.
Monitors hashrate, temperature and power usage + shows stats for Zcash price, network hashrate and difficulty.
Windows binary available at: https://www.dropbox.com/s/g16pbzd7gxgetgw/EWBF%20GUI.rar?dl=0.
Add conf.txt to folder for faster start up as without it program tries to find miner directory which is highly time consuming.

For running with python, required dependencies, that can be aquired with pip:
  - numpy
  - PyQt5
  - pyqtgraph
  - requests
  - psutils

Then run with: "python full.py". 
Tested with python 3.5.2

Usage:
  1. Select miner folder if not correct
  2. Insert the execution line normally used to launch miner. For monitoring you must use --api argument
  3. Click "Start mining", if willing to enable auto restart check the corresponding checkbox
  4. Set the update interval for graphing
  5. To start and observe graphs click "Start Monitor"
  6. Enjoy
  

Other notes for usage:
  - Minimum plotting interval should not be less than 30 s. That is same as update interval of EWBF miner
  - When mining is off slight lag is present while main window updates
  - For getting the miner information set the url that is used
  - conf.txt should be used in with script and the file consist following lines in order:
    - 1st line: miner folder
    - 2nd line: windows execution line
    - 3rd line: linux execution line
  
If you loose your mind and want to donate, mine with default execution line or send so ZEC address: t1dA2nN87SxyL4WYh1rWBaCWNqBiwNkpRGs
