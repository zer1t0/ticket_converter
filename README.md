# ticket_converter
A little tool to convert ccache tickets into kirbi (KRB-CRED) and vice versa based on impacket.

As input you must provide a ccache or kirbi file. The script will detect the format and convert it.

# Installation

```
git clone https://github.com/Zer1t0/ticket_converter
cd ticket_converter
pip install -r requirements.txt
```

# Usage

```
$ python ticket_converter.py -h
usage: ticket_converter.py [-h] input_file output_file

positional arguments:
  input_file
  output_file

optional arguments:
  -h, --help   show this help message and exit
```

Example:
```
$ python ticket_converter.py ticket.ccache ticket.kirbi
Converting kirbi => ccache
```

```
$ python ticket_converter.py ticket.kirbi ticket.ccache
Converting ccache => kirbi
```