
(英語が苦手なのでところどころ日本語で説明を書いています。)


## Background

[fpgasystems/fpga-network-stack](https://github.com/fpgasystems/fpga-network-stack)の成果を拝借してFPGA回路によるudpプロトコルスタックを作成する。  
TCPを除外したのは、再送制御などでメモリ量が必要になるため、実装が煩雑になるためである。



## Required

* KCU105 board
* Xilinx Vivado HLS 2018.3 (TODO : Update tool version)
* License of Xilinx 10Gbit Ethenet MAC IP (or Trimode Ethernet MAC IP)
	(TODO: Implement Trimode Ethernet MAC IP)
* MSYS2 environment on Windows 10
	make zip unzip


## Limitation

* Only UDP/IP (TCP/IP is not supported)
* Max packet size: 4096 byte (?)

