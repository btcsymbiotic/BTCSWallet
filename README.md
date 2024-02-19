Website :

https://crytposymbiotic.com

 Building ParsiPay (BTCS GUI Wallet) 

On *nix:

Dependencies: Git, GCC 4.7.3 or later (Visual Studio 2013 or later for windows), CMake 2.8.6 or later, Boost 1.55 or later and Qt5.

You may download them from:

http://microsoft.com/

http://gcc.gnu.org/

http://www.cmake.org/

http://www.boost.org/

http://www.qt.io/

Alternatively, it may be possible to install them using a package manager.

Build on *nix :


git clone https://github.com/btcsymbiotic/BTCSWallet.git && cd BTCSWallet && git clone https://github.com/btcsymbiotic/BTCSD.git cryptonote

sudo apt install qttools5-dev
sudo apt-get install qttools5-dev-tools
sudo apt-get install qt5-default


then : (tested on Ubuntu 16.04/18.04 & MAC OS X 10.12.6 with cmake 3.10.0 + GCC 7.3.0 + boost 1.67.0 + QT 5.11.1)


mkdir build && cd build && cmake -DBoost_USE_STATIC_LIBS=ON -DBoost_NO_BOOST_CMAKE=ON ..
 && make


on Windows:

git clone https://github.com/btcsymbiotic/BTCSWallet.git && cd BTCSWallet && git clone https://github.com/btcsymbiotic/BTCSD.git cryptonote

Then: (tested on windows 8.1/10 with boost 1.59.0 , cmake 3.10.0 , MSVS 2015 & Qt 5.11.3)


mkdir build && cd build && cmake .. -G "Visual Studio 14" -DCMAKE_PREFIX_PATH=C:\Qt\Qt5.11.3\5.11.3\msvc2015


then open ParsiPay.sln and Build.

Good luck!
