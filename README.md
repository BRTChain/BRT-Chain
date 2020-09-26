# BRT

Copyright (c) 2014-2020 The BRT Project.  
Portions Copyright (c) 2012-2013 The Cryptonote developers.

## Table of Contents

- [Development resources](#development-resources)
- [Vulnerability response](#vulnerability-response)
- [Research](#research)
- [Announcements](#announcements)
- [Translations](#translations)
- [Coverage](#coverage)
- [Introduction](#introduction)
- [About this project](#about-this-project)
- [Supporting the project](#supporting-the-project)
- [License](#license)
- [Contributing](#contributing)
- [Scheduled software upgrades](#scheduled-software-upgrades)
- [Release staging schedule and protocol](#release-staging-schedule-and-protocol)
- [Compiling BRT from source](#compiling-BRT-from-source)
  - [Dependencies](#dependencies)
- [Internationalization](#Internationalization)
- [Using Tor](#using-tor)
- [Pruning](#Pruning)
- [Debugging](#Debugging)
- [Known issues](#known-issues)

## Development resources

- GitHub: [https://github.com/BRTChain/BRT-Chain](https://github.com/BRTChain/BRT-Chain)
- IRC: [#BRT-dev on Freenode](https://webchat.freenode.net/?randomnick=1&channels=%23BRT-dev&prompt=1&uio=d4)
- It is HIGHLY recommended that you join the #BRT-dev IRC channel if you are developing software that uses BRT. Due to the nature of this open source software project, joining this channel and idling is the best way to stay updated on best practices and new developments in the BRT ecosystem. All you need to do is join the IRC channel and idle to stay updated with the latest in BRT development. If you do not, you risk wasting resources on developing integrations that are not compatible with the BRT network. The BRT core team and community continuously make efforts to communicate updates, developments, and documentation via other platforms – but for the best information, you need to talk to other BRT developers, and they are on IRC. #BRT-dev is about BRT development, not getting help about using BRT, or help about development of other software, including yours, unless it also pertains to BRT code itself. For these cases, checkout #BRT.

## Vulnerability response

- Our [Vulnerability Response Process](https://github.com/BRT-project/meta/blob/master/VULNERABILITY_RESPONSE_PROCESS.md) encourages responsible disclosure
- We are also available via [HackerOne](https://hackerone.com/BRT)

## Research

The [BRT Research Lab] is an open forum where the community coordinates research into BRT cryptography, protocols, fungibility, analysis, and more. We welcome collaboration and contributions from outside researchers! Because not all Lab work and publications are distributed as traditional preprints or articles, they may be easy to miss if you are conducting literature reviews for your own BRT research. You are encouraged to get in touch with our researchers if you have questions, wish to collaborate, or would like guidance to help avoid unnecessarily duplicating earlier or known work.

Our researchers are available on IRC in [#BRT-research-lab on Freenode](https://webchat.freenode.net/?randomnick=1&channels=%23BRT-research-lab&prompt=1&uio=d4) or by email:

- Larenk Maegther, Ph.D.
- Kurae Noser, Ph.D.

## Announcements

- You can subscribe to an [announcement listserv] to get critical announcements from the BRT core team. The announcement list can be very helpful for knowing when software updates are needed.

## Translations

The CLI wallet is available in different languages. If you want to help translate it, see our self-hosted localization platform. Every translation _must_ be uploaded on the platform, pull requests directly editing the code in this repository will be closed. If you need help with Weblate, you can find a guide with screenshots [here](https://github.com/BRTChain/BRT-Chain).
&nbsp;

If you need help/support/info about translations, contact the localization workgroup. You can find the complete list of contacts on the repository of the workgroup: [BRT-translations](https://github.com/BRT-ecosystem/BRT-translations#contacts).

## Coverage

| Type    | Status                                                                                                         |
| ------- | -------------------------------------------------------------------------------------------------------------- |
| License | [![License](https://img.shields.io/badge/license-BSD3-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) |

## Introduction

BRT is a private, secure, untraceable, decentralised digital currency. You are your bank, you control your funds, and nobody can trace your transfers unless you allow them to do so.

**Privacy:** BRT uses a cryptographically sound system to allow you to send and receive funds without your transactions being easily revealed on the blockchain (the ledger of transactions that everyone has). This ensures that your purchases, receipts, and all transfers remain absolutely private by default.

**Security:** Using the power of a distributed peer-to-peer consensus network, every transaction on the network is cryptographically secured. Individual wallets have a 25-word mnemonic seed that is only displayed once and can be written down to backup the wallet. Wallet files are encrypted with a passphrase to ensure they are useless if stolen.

**Untraceability:** By taking advantage of ring signatures, a special property of a certain type of cryptography, BRT is able to ensure that transactions are not only untraceable but have an optional measure of ambiguity that ensures that transactions cannot easily be tied back to an individual user or computer.

**Decentralization:** The utility of BRT depends on its decentralised peer-to-peer consensus network - anyone should be able to run the BRT software, validate the integrity of the blockchain, and participate in all aspects of the BRT network using consumer-grade commodity hardware. Decentralization of the BRT network is maintained by software development that minimizes the costs of running the BRT software and inhibits the proliferation of specialized, non-commodity hardware.

## About this project

This is the core implementation of BRT. It is open source and completely free to use without restrictions, except for those specified in the license agreement below. There are no restrictions on anyone creating an alternative implementation of BRT that uses the protocol and network in a compatible manner.

As with many development projects, the repository on Github is considered to be the "staging" area for the latest changes. Before changes are merged into that branch on the main repository, they are tested by individual developers in their own branches, submitted as a pull request, and then subsequently tested by contributors who focus on testing and code reviews. That having been said, the repository should be carefully considered before using it in a production environment, unless there is a patch in the repository for a particular show-stopping issue you are experiencing. It is generally a better idea to use a tagged release for stability.

**Anyone is welcome to contribute to BRT's codebase!** If you have a fix or code change, feel free to submit it as a pull request directly to the "master" branch. In cases where the change is relatively small or does not affect other parts of the codebase, it may be merged in immediately by any one of the collaborators. On the other hand, if the change is particularly large or complex, it is expected that it will be discussed at length either well in advance of the pull request being submitted, or even directly on the pull request.

## Supporting the project

BRT is a 100% community-sponsored endeavor. If you want to join our efforts, the easiest thing you can do is support the project financially. Both BRT and Bitcoin donations can be made to **donate.getBRT.org** if using a client that supports the [OpenAlias](https://openalias.org) standard. Alternatively, you can send BRT to the BRT donation address via the `donate` command (type `help` in the command-line wallet for details).

The BRT donation address is: `888tNkZrPN6JsEgekjMnABU4TBzc2Dt29EPAvkRxbANsAnjyPbb3iQ1YBRk1UXcdRsiKc9dhwMVgN5S9cQUiyoogDavup3H` (viewkey: `f359631075708155cc3d92a32b75a7d02a5dcf27756707b47a2b31b21c389501`)

The Bitcoin donation address is: `1KTexdemPdxSBcG55heUuTjDRYqbC5ZL8H`

Core development funding and/or some supporting services are also graciously provided by sponsors.

There are also several mining pools that kindly donate a portion of their fees, [a list of them can be found on our Bitcointalk post](https://github.com/BRTChain/BRT-Chain).

## License

See [LICENSE](LICENSE).

## Contributing

If you want to help out, see [CONTRIBUTING](CONTRIBUTING.md) for a set of guidelines.

## Scheduled software upgrades

BRT uses a fixed-schedule software upgrade (hard fork) mechanism to implement new features. This means that users of BRT (end users and service providers) should run current versions and upgrade their software on a regular schedule. Software upgrades occur during the months of April and October. The required software for these upgrades will be available prior to the scheduled date. Please check the repository prior to this date for the proper BRT software version. Below is the historical schedule and the projected schedule for the next upgrade.
Dates are provided in the format YYYY-MM-DD.

| Software upgrade block height | Date       | Fork version | Minimum BRT version | Recommended BRT version | Details                                                                     |
| ----------------------------- | ---------- | ------------ | ------------------- | ----------------------- | --------------------------------------------------------------------------- |
| 1009827                       | 2020-09-28 | v2           | v0.9.4              | v0.9.4                  | Allow only >= ringsize 3, blocktime = 120 seconds, fee-free blocksize 60 kb |
| XXXXXXX                       | XXX-XX-XX  | XXX          | vX.XX.X.X           | vX.XX.X.X               | XXX                                                                         |

X's indicate that these details have not been determined as of commit date.

\* indicates estimate as of commit date

## Release staging schedule and protocol

Approximately three months prior to a scheduled software upgrade, a branch from master will be created with the new release version tag. Pull requests that address bugs should then be made to both master and the new release branch. Pull requests that require extensive review and testing (generally, optimizations and new features) should _not_ be made to the release branch.

## Compiling BRT from source

### Dependencies

The following table summarizes the tools and libraries required to build. A
few of the libraries are also included in this repository (marked as
"Vendored"). By default, the build uses the library installed on the system
and ignores the vendored sources. However, if no library is found installed on
the system, then the vendored source will be built and used. The vendored
sources are also used for statically-linked builds because distribution
packages often include only shared library binaries (`.so`) but not static
library archives (`.a`).

| Dep         | Min. version  | Vendored | Debian/Ubuntu pkg    | Arch pkg     | Void pkg              | Fedora pkg          | Optional | Purpose         |
| ----------- | ------------- | -------- | -------------------- | ------------ | --------------------- | ------------------- | -------- | --------------- |
| GCC         | 4.7.3         | NO       | `build-essential`    | `base-devel` | `base-devel`          | `gcc`               | NO       |                 |
| CMake       | 3.5           | NO       | `cmake`              | `cmake`      | `cmake`               | `cmake`             | NO       |                 |
| pkg-config  | any           | NO       | `pkg-config`         | `base-devel` | `base-devel`          | `pkgconf`           | NO       |                 |
| Boost       | 1.58          | NO       | `libboost-all-dev`   | `boost`      | `boost-devel`         | `boost-devel`       | NO       | C++ libraries   |
| OpenSSL     | basically any | NO       | `libssl-dev`         | `openssl`    | `libressl-devel`      | `openssl-devel`     | NO       | sha256 sum      |
| libzmq      | 3.0.0         | NO       | `libzmq3-dev`        | `zeromq`     | `zeromq-devel`        | `zeromq-devel`      | NO       | ZeroMQ library  |
| OpenPGM     | ?             | NO       | `libpgm-dev`         | `libpgm`     |                       | `openpgm-devel`     | NO       | For ZeroMQ      |
| libnorm[2]  | ?             | NO       | `libnorm-dev`        |              |                       |                     | YES      | For ZeroMQ      |
| libunbound  | 1.4.16        | YES      | `libunbound-dev`     | `unbound`    | `unbound-devel`       | `unbound-devel`     | NO       | DNS resolver    |
| libsodium   | ?             | NO       | `libsodium-dev`      | `libsodium`  | `libsodium-devel`     | `libsodium-devel`   | NO       | cryptography    |
| libunwind   | any           | NO       | `libunwind8-dev`     | `libunwind`  | `libunwind-devel`     | `libunwind-devel`   | YES      | Stack traces    |
| liblzma     | any           | NO       | `liblzma-dev`        | `xz`         | `liblzma-devel`       | `xz-devel`          | YES      | For libunwind   |
| libreadline | 6.3.0         | NO       | `libreadline6-dev`   | `readline`   | `readline-devel`      | `readline-devel`    | YES      | Input editing   |
| ldns        | 1.6.17        | NO       | `libldns-dev`        | `ldns`       | `libldns-devel`       | `ldns-devel`        | YES      | SSL toolkit     |
| expat       | 1.1           | NO       | `libexpat1-dev`      | `expat`      | `expat-devel`         | `expat-devel`       | YES      | XML parsing     |
| GTest       | 1.5           | YES      | `libgtest-dev`[1]    | `gtest`      | `gtest-devel`         | `gtest-devel`       | YES      | Test suite      |
| Doxygen     | any           | NO       | `doxygen`            | `doxygen`    | `doxygen`             | `doxygen`           | YES      | Documentation   |
| Graphviz    | any           | NO       | `graphviz`           | `graphviz`   | `graphviz`            | `graphviz`          | YES      | Documentation   |
| lrelease    | ?             | NO       | `qttools5-dev-tools` | `qt5-tools`  | `qt5-tools`           | `qt5-linguist`      | YES      | Translations    |
| libhidapi   | ?             | NO       | `libhidapi-dev`      | `hidapi`     | `hidapi-devel`        | `hidapi-devel`      | YES      | Hardware wallet |
| libusb      | ?             | NO       | `libusb-1.0-0-dev`   | `libusb`     | `libusb-devel`        | `libusbx-devel`     | YES      | Hardware wallet |
| libprotobuf | ?             | NO       | `libprotobuf-dev`    | `protobuf`   | `protobuf-devel`      | `protobuf-devel`    | YES      | Hardware wallet |
| protoc      | ?             | NO       | `protobuf-compiler`  | `protobuf`   | `protobuf`            | `protobuf-compiler` | YES      | Hardware wallet |
| libudev     | ?             | No       | `libudev-dev`        | `systemd`    | `eudev-libudev-devel` | `systemd-devel`     | YES      | Hardware wallet |

[1] On Debian/Ubuntu `libgtest-dev` only includes sources and headers. You must
build the library binary manually. This can be done with the following command `sudo apt-get install libgtest-dev && cd /usr/src/gtest && sudo cmake . && sudo make && sudo mv libg* /usr/lib/ `
[2] libnorm-dev is needed if your zmq library was built with libnorm, and not needed otherwise

Install all dependencies at once on Debian/Ubuntu:

` sudo apt update && sudo apt install build-essential cmake pkg-config libboost-all-dev libssl-dev libzmq3-dev libunbound-dev libsodium-dev libunwind8-dev liblzma-dev libreadline6-dev libldns-dev libexpat1-dev doxygen graphviz libpgm-dev qttools5-dev-tools libhidapi-dev libusb-1.0-0-dev libprotobuf-dev protobuf-compiler libudev-dev`

Install all dependencies at once on macOS with the provided Brewfile:
`brew update && brew bundle --file=contrib/brew/Brewfile`

FreeBSD 12.1 one-liner required to build dependencies:
`pkg install git gmake cmake pkgconf boost-libs libzmq4 libsodium`

### Cloning the repository

Clone recursively to pull-in needed submodule(s):

`$ git clone --recursive https://github.com/BRTChain/BRT-Chain`

If you already have a repo cloned, initialize and update:

`$ cd BRT && git submodule init && git submodule update`

### Build instructions

BRT uses the CMake build system and a top-level [Makefile](Makefile) that
invokes cmake commands as needed.

#### On Linux and macOS

- Install the dependencies
- Change to the root of the source code directory, change to the most recent release branch, and build:

  ```bash
  cd BRT
  git checkout release-v0.17
  make
  ```

  _Optional_: If your machine has several cores and enough memory, enable
  parallel build by running `make -j<number of threads>` instead of `make`. For
  this to be worthwhile, the machine should have one core and about 2GB of RAM
  available per thread.

  _Note_: The instructions above will compile the most stable release of the
  BRT software. If you would like to use and test the most recent software,
  use `git checkout master`. The master branch may contain updates that are
  both unstable and incompatible with release software, though testing is always
  encouraged.

- The resulting executables can be found in `build/release/bin`

- Add `PATH="$PATH:$HOME/BRT/build/release/bin"` to `.profile`

- Run BRT with `BRTd --detach`

- **Optional**: build and run the test suite to verify the binaries:

  ```bash
  make release-test
  ```

  _NOTE_: `core_tests` test may take a few hours to complete.

- **Optional**: to build binaries suitable for debugging:

  ```bash
  make debug
  ```

- **Optional**: to build statically-linked binaries:

  ```bash
  make release-static
  ```

Dependencies need to be built with -fPIC. Static libraries usually aren't, so you may have to build them yourself with -fPIC. Refer to their documentation for how to build them.

- **Optional**: build documentation in `doc/html` (omit `HAVE_DOT=YES` if `graphviz` is not installed):

  ```bash
  HAVE_DOT=YES doxygen Doxyfile
  ```

#### On the Raspberry Pi

Tested on a Raspberry Pi Zero with a clean install of minimal Raspbian Stretch (2017-09-07 or later) from https://www.raspberrypi.org/downloads/raspbian/. If you are using Raspian Jessie, [please see note in the following section](#note-for-raspbian-jessie-users).

- `apt-get update && apt-get upgrade` to install all of the latest software

- Install the dependencies for BRT from the 'Debian' column in the table above.

- Increase the system swap size:

  ```bash
  sudo /etc/init.d/dphys-swapfile stop
  sudo nano /etc/dphys-swapfile
  CONF_SWAPSIZE=2048
  sudo /etc/init.d/dphys-swapfile start
  ```

- If using an external hard disk without an external power supply, ensure it gets enough power to avoid hardware issues when syncing, by adding the line "max_usb_current=1" to /boot/config.txt

- Clone BRT and checkout the most recent release version:

  ```bash
  git clone https://github.com/BRTChain/BRT-Chain.git
  cd BRT
  ```

- Build:

  ```bash
  make release
  ```

- Wait 4-6 hours

- The resulting executables can be found in `build/release/bin`

- Add `PATH="$PATH:$HOME/BRT/build/release/bin"` to `.profile`

- Run BRT with `BRTd --detach`

- You may wish to reduce the size of the swap file after the build has finished, and delete the boost directory from your home directory

#### _Note for Raspbian Jessie users:_

If you are using the older Raspbian Jessie image, compiling BRT is a bit more complicated. The version of Boost available in the Debian Jessie repositories is too old to use with BRT, and thus you must compile a newer version yourself. The following explains the extra steps and has been tested on a Raspberry Pi 2 with a clean install of minimal Raspbian Jessie.

- As before, `apt-get update && apt-get upgrade` to install all of the latest software, and increase the system swap size

  ```bash
  sudo /etc/init.d/dphys-swapfile stop
  sudo nano /etc/dphys-swapfile
  CONF_SWAPSIZE=2048
  sudo /etc/init.d/dphys-swapfile start
  ```

- Then, install the dependencies for BRT except for `libunwind` and `libboost-all-dev`

- Install the latest version of boost (this may first require invoking `apt-get remove --purge libboost*-dev` to remove a previous version if you're not using a clean install):

  ```bash
  cd
  wget https://sourceforge.net/projects/boost/files/boost/1.72.0/boost_1_72_0.tar.bz2
  tar xvfo boost_1_72_0.tar.bz2
  cd boost_1_72_0
  ./bootstrap.sh
  sudo ./b2
  ```

- Wait ~8 hours

  ```bash
  sudo ./bjam cxxflags=-fPIC cflags=-fPIC -a install
  ```

- Wait ~4 hours

- From here, follow the [general Raspberry Pi instructions](#on-the-raspberry-pi) from the "Clone BRT and checkout most recent release version" step.

#### On Windows:

Binaries for Windows are built on Windows using the MinGW toolchain within
[MSYS2 environment](https://www.msys2.org). The MSYS2 environment emulates a
POSIX system. The toolchain runs within the environment and _cross-compiles_
binaries that can run outside of the environment as a regular Windows
application.

**Preparing the build environment**

- Download and install the [MSYS2 installer](https://www.msys2.org), either the 64-bit or the 32-bit package, depending on your system.
- Open the MSYS shell via the `MSYS2 Shell` shortcut
- Update packages using pacman:

  ```bash
  pacman -Syu
  ```

- Exit the MSYS shell using Alt+F4
- Edit the properties for the `MSYS2 Shell` shortcut changing "msys2_shell.bat" to "msys2_shell.cmd -mingw64" for 64-bit builds or "msys2_shell.cmd -mingw32" for 32-bit builds
- Restart MSYS shell via modified shortcut and update packages again using pacman:

  ```bash
  pacman -Syu
  ```

- Install dependencies:

  To build for 64-bit Windows:

  ```bash
  pacman -S mingw-w64-x86_64-toolchain make mingw-w64-x86_64-cmake mingw-w64-x86_64-boost mingw-w64-x86_64-openssl mingw-w64-x86_64-zeromq mingw-w64-x86_64-libsodium mingw-w64-x86_64-hidapi
  ```

  To build for 32-bit Windows:

  ```bash
  pacman -S mingw-w64-i686-toolchain make mingw-w64-i686-cmake mingw-w64-i686-boost mingw-w64-i686-openssl mingw-w64-i686-zeromq mingw-w64-i686-libsodium mingw-w64-i686-hidapi
  ```

- Open the MingW shell via `MinGW-w64-Win64 Shell` shortcut on 64-bit Windows
  or `MinGW-w64-Win64 Shell` shortcut on 32-bit Windows. Note that if you are
  running 64-bit Windows, you will have both 64-bit and 32-bit MinGW shells.

**Cloning**

- To git clone, run:

  ```bash
  git clone --recursive https://github.com/BRT-project/BRT.git
  ```

**Building**

- Change to the cloned directory, run:

  ```bash
  cd BRT
  ```

- If you would like a specific [version/tag](https://github.com/BRT-project/BRT/tags), do a git checkout for that version. eg. 'v0.17.0.0'. If you don't care about the version and just want binaries from master, skip this step:

  ```bash
  git checkout v0.17.0.0
  ```

- If you are on a 64-bit system, run:

  ```bash
  make release-static-win64
  ```

- If you are on a 32-bit system, run:

  ```bash
  make release-static-win32
  ```

- The resulting executables can be found in `build/release/bin`

- **Optional**: to build Windows binaries suitable for debugging on a 64-bit system, run:

  ```bash
  make debug-static-win64
  ```

- **Optional**: to build Windows binaries suitable for debugging on a 32-bit system, run:

  ```bash
  make debug-static-win32
  ```

- The resulting executables can be found in `build/debug/bin`

### On FreeBSD:

The project can be built from scratch by following instructions for Linux above(but use `gmake` instead of `make`).
If you are running BRT in a jail, you need to add `sysvsem="new"` to your jail configuration, otherwise lmdb will throw the error message: `Failed to open lmdb environment: Function not implemented`.

BRT is also available as a port or package as 'BRT-cli`.

### On OpenBSD:

You will need to add a few packages to your system. `pkg_add cmake gmake zeromq libiconv boost`.

The `doxygen` and `graphviz` packages are optional and require the xbase set.
Running the test suite also requires `py-requests` package.

Build BRT: `env DEVELOPER_LOCAL_TOOLS=1 BOOST_ROOT=/usr/local gmake release-static`

Note: you may encounter the following error when compiling the latest version of BRT as a normal user:

```
LLVM ERROR: out of memory
c++: error: unable to execute command: Abort trap (core dumped)
```

Then you need to increase the data ulimit size to 2GB and try again: `ulimit -d 2000000`

### On NetBSD:

Check that the dependencies are present: `pkg_info -c libexecinfo boost-headers boost-libs protobuf readline libusb1 zeromq git-base pkgconf gmake cmake | more`, and install any that are reported missing, using `pkg_add` or from your pkgsrc tree. Readline is optional but worth having.

Third-party dependencies are usually under `/usr/pkg/`, but if you have a custom setup, adjust the "/usr/pkg" (below) accordingly.

Clone the BRT repository recursively and checkout the most recent release as described above. Then build BRT: `gmake BOOST_ROOT=/usr/pkg LDFLAGS="-Wl,-R/usr/pkg/lib" release`. The resulting executables can be found in `build/NetBSD/[Release version]/Release/bin/`.

### On Solaris:

The default Solaris linker can't be used, you have to install GNU ld, then run cmake manually with the path to your copy of GNU ld:

```bash
mkdir -p build/release
cd build/release
cmake -DCMAKE_LINKER=/path/to/ld -D CMAKE_BUILD_TYPE=Release ../..
cd ../..
```

Then you can run make as usual.

### On Linux for Android (using docker):

```bash
# Build image (for ARM 32-bit)
docker build -f utils/build_scripts/android32.Dockerfile -t BRT-android .
# Build image (for ARM 64-bit)
docker build -f utils/build_scripts/android64.Dockerfile -t BRT-android .
# Create container
docker create -it --name BRT-android BRT-android bash
# Get binaries
docker cp BRT-android:/src/build/release/bin .
```

### Building portable statically linked binaries

By default, in either dynamically or statically linked builds, binaries target the specific host processor on which the build happens and are not portable to other processors. Portable binaries can be built using the following targets:

- `make release-static-linux-x86_64` builds binaries on Linux on x86_64 portable across POSIX systems on x86_64 processors
- `make release-static-linux-i686` builds binaries on Linux on x86_64 or i686 portable across POSIX systems on i686 processors
- `make release-static-linux-armv8` builds binaries on Linux portable across POSIX systems on armv8 processors
- `make release-static-linux-armv7` builds binaries on Linux portable across POSIX systems on armv7 processors
- `make release-static-linux-armv6` builds binaries on Linux portable across POSIX systems on armv6 processors
- `make release-static-win64` builds binaries on 64-bit Windows portable across 64-bit Windows systems
- `make release-static-win32` builds binaries on 64-bit or 32-bit Windows portable across 32-bit Windows systems

### Cross Compiling

You can also cross-compile static binaries on Linux for Windows and macOS with the `depends` system.

- `make depends target=x86_64-linux-gnu` for 64-bit linux binaries.
- `make depends target=x86_64-w64-mingw32` for 64-bit windows binaries.
  - Requires: `python3 g++-mingw-w64-x86-64 wine1.6 bc`
- `make depends target=x86_64-apple-darwin11` for macOS binaries.
  - Requires: `cmake imagemagick libcap-dev librsvg2-bin libz-dev libbz2-dev libtiff-tools python-dev`
- `make depends target=i686-linux-gnu` for 32-bit linux binaries.
  - Requires: `g++-multilib bc`
- `make depends target=i686-w64-mingw32` for 32-bit windows binaries.
  - Requires: `python3 g++-mingw-w64-i686`
- `make depends target=arm-linux-gnueabihf` for armv7 binaries.
  - Requires: `g++-arm-linux-gnueabihf`
- `make depends target=aarch64-linux-gnu` for armv8 binaries.
  - Requires: `g++-aarch64-linux-gnu`
- `make depends target=riscv64-linux-gnu` for RISC V 64 bit binaries.
  - Requires: `g++-riscv64-linux-gnu`
- `make depends target=x86_64-unknown-freebsd` for freebsd binaries.
  - Requires: `clang-8`
- `make depends target=arm-linux-android` for 32bit android binaries
- `make depends target=aarch64-linux-android` for 64bit android binaries

The required packages are the names for each toolchain on apt. Depending on your distro, they may have different names.

Using `depends` might also be easier to compile BRT on Windows than using MSYS. Activate Windows Subsystem for Linux (WSL) with a distro (for example Ubuntu), install the apt build-essentials and follow the `depends` steps as depicted above.

The produced binaries still link libc dynamically. If the binary is compiled on a current distribution, it might not run on an older distribution with an older installation of libc. Passing `-DBACKCOMPAT=ON` to cmake will make sure that the binary will run on systems having at least libc version 2.17.

## Installing BRT from a package

**DISCLAIMER: These packages are not part of this repository or maintained by this project's contributors, and as such, do not go through the same review process to ensure their trustworthiness and security.**

Packages are available for

- Debian Buster

  See the [instructions in the whonix/BRT-gui repository](https://gitlab.com/whonix/BRT-gui#how-to-install-BRT-using-apt-get)

- Debian Bullseye and Sid

      ```bash
      sudo apt install BRT
      ```

  More info and versions in the [Debian package tracker](https://tracker.debian.org/pkg/BRT).

- Arch Linux (via Community packages):
  [`BRT`](https://www.archlinux.org/packages/community/x86_64/BRT/)

- Void Linux:

  ```bash
  xbps-install -S BRT
  ```

- GuixSD

  ```bash
  guix package -i BRT
  ```

- Gentoo [BRT overlay](https://github.com/gentoo-BRT/gentoo-BRT)

  ```bash
  emerge --noreplace eselect-repository
  eselect repository enable BRT
  emaint sync -r BRT
  echo '*/*::BRT ~amd64' >> /etc/portage/package.accept_keywords
  emerge net-p2p/BRT
  ```

- macOS (homebrew)

  ```bash
  brew install BRT
  ```

- Docker

  ```bash
  # Build using all available cores
  docker build -t BRT .

  # or build using a specific number of cores (reduce RAM requirement)
  docker build --build-arg NPROC=1 -t BRT .

  # either run in foreground
  docker run -it -v /BRT/chain:/root/.bitBRT -v /BRT/wallet:/wallet -p 18080:18080 BRT

  # or in background
  docker run -it -d -v /BRT/chain:/root/.bitBRT -v /BRT/wallet:/wallet -p 18080:18080 BRT
  ```

- The build needs 3 GB space.
- Wait one hour or more

Packaging for your favorite distribution would be a welcome contribution!

## Running BRTd

The build places the binary in `bin/` sub-directory within the build directory
from which cmake was invoked (repository root by default). To run in the
foreground:

```bash
./bin/BRTd
```

To list all available options, run `./bin/BRTd --help`. Options can be
specified either on the command line or in a configuration file passed by the
`--config-file` argument. To specify an option in the configuration file, add
a line with the syntax `argumentname=value`, where `argumentname` is the name
of the argument without the leading dashes, for example, `log-level=1`.

To run in background:

```bash
./bin/BRTd --log-file BRTd.log --detach
```

To run as a systemd service, copy
[BRTd.service](utils/systemd/BRTd.service) to `/etc/systemd/system/` and
[BRTd.conf](utils/conf/BRTd.conf) to `/etc/`. The [example
service](utils/systemd/BRTd.service) assumes that the user `BRT` exists
and its home is the data directory specified in the [example
config](utils/conf/BRTd.conf).

If you're on Mac, you may need to add the `--max-concurrency 1` option to
BRT-wallet-cli, and possibly BRTd, if you get crashes refreshing.

## Internationalization

See [README.i18n.md](README.i18n.md).

## Using Tor

> There is a new, still experimental, [integration with Tor](ANONYMITY_NETWORKS.md). The
> feature allows connecting over IPv4 and Tor simultaneously - IPv4 is used for
> relaying blocks and relaying transactions received by peers whereas Tor is
> used solely for relaying transactions received over local RPC. This provides
> privacy and better protection against surrounding node (sybil) attacks.

While BRT isn't made to integrate with Tor, it can be used wrapped with torsocks, by
setting the following configuration parameters and environment variables:

- `--p2p-bind-ip 127.0.0.1` on the command line or `p2p-bind-ip=127.0.0.1` in
  BRTd.conf to disable listening for connections on external interfaces.
- `--no-igd` on the command line or `no-igd=1` in BRTd.conf to disable IGD
  (UPnP port forwarding negotiation), which is pointless with Tor.
- `DNS_PUBLIC=tcp` or `DNS_PUBLIC=tcp://x.x.x.x` where x.x.x.x is the IP of the
  desired DNS server, for DNS requests to go over TCP, so that they are routed
  through Tor. When IP is not specified, BRTd uses the default list of
  servers defined in [src/common/dns_utils.cpp](src/common/dns_utils.cpp).
- `TORSOCKS_ALLOW_INBOUND=1` to tell torsocks to allow BRTd to bind to interfaces
  to accept connections from the wallet. On some Linux systems, torsocks
  allows binding to localhost by default, so setting this variable is only
  necessary to allow binding to local LAN/VPN interfaces to allow wallets to
  connect from remote hosts. On other systems, it may be needed for local wallets
  as well.
- Do NOT pass `--detach` when running through torsocks with systemd, (see
  [utils/systemd/BRTd.service](utils/systemd/BRTd.service) for details).
- If you use the wallet with a Tor daemon via the loopback IP (eg, 127.0.0.1:9050),
  then use `--untrusted-daemon` unless it is your own hidden service.

Example command line to start BRTd through Tor:

```bash
DNS_PUBLIC=tcp torsocks BRTd --p2p-bind-ip 127.0.0.1 --no-igd
```

### Using Tor on Tails

TAILS ships with a very restrictive set of firewall rules. Therefore, you need
to add a rule to allow this connection too, in addition to telling torsocks to
allow inbound connections. Full example:

```bash
sudo iptables -I OUTPUT 2 -p tcp -d 127.0.0.1 -m tcp --dport 18081 -j ACCEPT
DNS_PUBLIC=tcp torsocks ./BRTd --p2p-bind-ip 127.0.0.1 --no-igd --rpc-bind-ip 127.0.0.1 \
    --data-dir /home/amnesia/Persistent/your/directory/to/the/blockchain
```

## Pruning

As of May 2020, the full BRT blockchain file is about 80 GB. One can store a pruned blockchain, which is about 28 GB.
A pruned blockchain can only serve part of the historical chain data to other peers, but is otherwise identical in
functionality to the full blockchain.
To use a pruned blockchain, it is best to start the initial sync with --prune-blockchain. However, it is also possible
to prune an existing blockchain using the BRT-blockchain-prune tool or using the --prune-blockchain BRTd option
with an existing chain. If an existing chain exists, pruning will temporarily require disk space to store both the full
and pruned blockchains.

## Debugging

This section contains general instructions for debugging failed installs or problems encountered with BRT. First, ensure you are running the latest version built from the Github repo.

### Obtaining stack traces and core dumps on Unix systems

We generally use the tool `gdb` (GNU debugger) to provide stack trace functionality, and `ulimit` to provide core dumps in builds which crash or segfault.

- To use `gdb` in order to obtain a stack trace for a build that has stalled:

Run the build.

Once it stalls, enter the following command:

```bash
gdb /path/to/BRTd `pidof BRTd`
```

Type `thread apply all bt` within gdb in order to obtain the stack trace

- If however the core dumps or segfaults:

Enter `ulimit -c unlimited` on the command line to enable unlimited filesizes for core dumps

Enter `echo core | sudo tee /proc/sys/kernel/core_pattern` to stop cores from being hijacked by other tools

Run the build.

When it terminates with an output along the lines of "Segmentation fault (core dumped)", there should be a core dump file in the same directory as BRTd. It may be named just `core`, or `core.xxxx` with numbers appended.

You can now analyse this core dump with `gdb` as follows:

```bash
gdb /path/to/BRTd /path/to/dumpfile`
```

Print the stack trace with `bt`

- If a program crashed and cores are managed by systemd, the following can also get a stack trace for that crash:

```bash
coredumpctl -1 gdb
```

#### To run BRT within gdb:

Type `gdb /path/to/BRTd`

Pass command-line options with `--args` followed by the relevant arguments

Type `run` to run BRTd

### Analysing memory corruption

There are two tools available:

#### ASAN

Configure BRT with the -D SANITIZE=ON cmake flag, eg:

```bash
cd build/debug && cmake -D SANITIZE=ON -D CMAKE_BUILD_TYPE=Debug ../..
```

You can then run the BRT tools normally. Performance will typically halve.

#### valgrind

Install valgrind and run as `valgrind /path/to/BRTd`. It will be very slow.

### LMDB

Instructions for debugging suspected blockchain corruption as per @HYC

There is an `mdb_stat` command in the LMDB source that can print statistics about the database but it's not routinely built. This can be built with the following command:

```bash
cd ~/BRT/external/db_drivers/liblmdb && make
```

The output of `mdb_stat -ea <path to blockchain dir>` will indicate inconsistencies in the blocks, block_heights and block_info table.

The output of `mdb_dump -s blocks <path to blockchain dir>` and `mdb_dump -s block_info <path to blockchain dir>` is useful for indicating whether blocks and block_info contain the same keys.

These records are dumped as hex data, where the first line is the key and the second line is the data.

# Known Issues

## Protocols

### Socket-based

Because of the nature of the socket-based protocols that drive BRT, certain protocol weaknesses are somewhat unavoidable at this time. While these weaknesses can theoretically be fully mitigated, the effort required (the means) may not justify the ends. As such, please consider taking the following precautions if you are a BRT node operator:

- Run `BRTd` on a "secured" machine. If operational security is not your forte, at a very minimum, have a dedicated a computer running `BRTd` and **do not** browse the web, use email clients, or use any other potentially harmful apps on your `BRTd` machine. **Do not click links or load URL/MUA content on the same machine**. Doing so may potentially exploit weaknesses in commands which accept "localhost" and "127.0.0.1".
- If you plan on hosting a public "remote" node, start `BRTd` with `--restricted-rpc`. This is a must.

### Blockchain-based

Certain blockchain "features" can be considered "bugs" if misused correctly. Consequently, please consider the following:

- When receiving BRT, be aware that it may be locked for an arbitrary time if the sender elected to, preventing you from spending that BRT until the lock time expires. You may want to hold off acting upon such a transaction until the unlock time lapses. To get a sense of that time, you can consider the remaining blocktime until unlock as seen in the `show_transfers` command.
