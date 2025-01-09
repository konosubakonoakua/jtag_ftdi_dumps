# ftdi_dumps

It looks like Xilinx finally added a [tool](https://docs.xilinx.com/r/en-US/ug908-vivado-programming-debugging/JTAG-Cables-and-Devices-Supported-by-hw_server) to convert any FT232H, FT2232H, or FT4232H to a supported programmer in Vivado. As such, this repo is being archived.

FTDI EEPROM dumps for common JTAG FPGA programmers mostly pulled from https://gist.github.com/rikka0w0/24b58b54473227502fa0334bbe75c3c1. To flash a binary, run the following command.

	sudo ftdi_eeprom --flash-eeprom <config-file>

| conf file | chip | status |
| --- | --- | --- |
| digilent_hs2.conf | FT232H | not tested |
| arrow_ftdi.conf | FT2232H | not working with vivado 2019.1 on linux, working on win |
| digilent_smt1.conf | FT2232H | working well |
| pynqz2_ftdi.conf | FT2232H | not working with vivado 2019.1 on linux, working on win |
| ft4232h.conf | FT4232H | not tested |
