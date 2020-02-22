# Welcome to GLX!

GLX is a decentralized supercomputer based on cryptography and blockchain technology.

----
## disclaimer

GLX IS OPEN-SOURCE SOFTWARE RUNNING ON THE TEST-NET BUT IS STILL CONSIDERED "ALPHA" AND MAY CONTAIN BUGS, SOME OF WHICH MAY HAVE SERIOUS CONSEQUENCES. WE THEREFORE DISCLAIM ANY LIABILITY OF ANY KIND FOR ANY DAMAGES WHATSOEVER RESULTING DIRECTLY OR INDIRECTLY FROM THE USE OF THIS SOFTWARE OR OF ANY DERIVATIVE WORK. USE THE SOFTWARE AND THE INFORMATION PRESENTED HERE AT OUR OWN RISK.

----
## Run GLX Computation Wallet from sources (***recommended for advanced users***)

### dependencies
  - Java 12 : [oracle jdk](https://www.oracle.com/technetwork/java/javase/downloads/jdk12-downloads-5295953.html) or [openjdk](https://jdk.java.net/12/)
  - Maven : https://maven.apache.org/install.html

### clone the repository

```
git clone https://github.com/tieandsuit/GLX
cd GLX
```

### compile it

`mvn package`

### clone the miner

clone the miner next to your wallet folder like this :

```
my_main_folder/GLX
my_main_folder/glx-miner
```

```
git clone https://github.com/xel-software/xel-miner
cd glx-miner
cmake .
make install
```

### integrate the miner into the computation wallet

```
cd GLX
./pull_miner.sh
```

### start from the command line:
- Linux/macOS: `./start.sh`
- Windows: `run.bat`


***wait for the JavaFX wallet window to open***
***on platforms without JavaFX, open http://localhost:16876/ in a browser***
