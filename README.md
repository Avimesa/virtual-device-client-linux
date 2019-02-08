# Avimesa Virtual Device Client (x86_64)

This project contains an Avimesa Virtual Device Client for Linux in a binary form (x86_64) that can be ran from command line.

- [1. Overview](#1.-overview)
- [2. Prerequisites](#2.-prerequisites)
- [3. Usage](#3.-usage)

<a id="1.-overview"></a>
## 1. Overview

The Avimesa Virtual Device Client (VDC) allows one to easily use a Client on most Linux distributions to simulate or even implement devices.

Using the VDC, one can fully utilize the Avimesa Device Cloud from a Linux command line with JSON.

<a id="2.-prerequisites"></a>
## 2. Prerequisites

- A valid Avimesa Device Cloud Device ID and Authentication Key
- A Linux Host (x86_64, Debian, CentOS, RHEL7, kernel 3.10+) with internet access
- Text editor to modify a JSON file

<a id="3.-usage"></a>
## 3. Usage

Checkout the client:
```
git clone https://github.com/Avimesa/virtual-device-client-linux.git
cd virtual-device-client-linux
```

Run via command line, where you need to provide a valid Device ID (-i) and Authentication Key (-a)
```
./avmsavdc -s 64.40.116.246 -p 36360 -j data.json -i 00000000000000000000000000000000 -a 11111111111111111111111111111111
```

If successful, you'll get a JSON response.  If no response, there is likely an issue with the Device ID and Authentication Key.
