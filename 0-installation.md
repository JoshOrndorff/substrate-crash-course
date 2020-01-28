Installation
============

The videos in this course will be recorded on a Debian-based linux system. The installation will look somewhat different on Mac, or Linux. However, after installation is complete, the development process will be similar regardless of platform.

!!! TODO insert video here.


## Install Substrate Dependencies

```bash
$ curl https://getsubstrate.io -sSf | bash -s -- --fast
```

Note: Windows users can follow the instructions found here: https://substrate.dev/docs/en/next/getting-started#getting-started-on-windows

## Clone Substrate Node Template

```bash
$ git clone https://github.com/substrate-developer-hub/substrate-node-template
```

## Build the Substrate Node Template

```bash
cd substrate-node-template/
$ cargo build --release
```

## Test Run Your Node

If everything worked successfully, you should be able to display the node template's help text.

```bash
$ ./target/release/node-template --help

node-template 2.0.0-x86_64-linux-gnu

Anonymous
Template Node

USAGE:
    node-template [FLAGS] [OPTIONS]
    node-template <SUBCOMMAND>
...
```


## A Note on Windows

For learners using Windows, it will be easiest to follow this course by using the Windows Subsystem for Linux.

Manual [instructions for Windows](https://substrate.dev/docs/en/getting-started/installing-substrate#windows) are also available to run natively. Although Windows is a supported platform for Substrate and Polkadot, it will only be supported on a best-effort basis for this course, at least initially.
