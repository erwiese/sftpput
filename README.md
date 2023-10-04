# tinysftp: minimalistic SFTP client program and library

This SFTP client can be usefull especially on old operating systems, with old SSH libraries, that do not provide modern ciphers, MACs etc and common tools like scp or sftp may not work.
Only the most important features are implemented:
* ls 
* get
* put

# Update Oct-2023: 
Use https://github.com/melbahja/goph with a lot more features

## Installation

Make sure you have a working Go environment. [See
the install instructions for Go](http://golang.org/doc/install.html).

To install the command-line client:
```
# clone the project: 
git clone https://github.com/erwiese/tinysftp.git

cd tinysftp
go build|install
```

Import library:
```
$ go get github.com/erwiese/tinysftp
```

## Usage
```
export SFTPGO_URL=sftp://[user:pw@]host[:port]

tinysftp --help

# Command help
tinysftp put --help
```
