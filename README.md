# Oregano

MITM proxy for Tor. We can bootstrap a Tor client to 100% now.

## Usage

Edit `configuration.py` under directory `oregano` for configuration and run module `oregano.proxy`.
```
python -m oregano.proxy
```

Then set `UseBridges` or use a Tor controller to instruct a Tor client to connect to the listening interface.
```
UseBridges 1
Bridge 127.0.0.1:40056
```

## Dependencies

* Python 2.7
* [GnuTLS](https://gnutls.org/)
* [python-gnutls](https://github.com/AGProjects/python-gnutls)
* [PyCryptodome](https://www.pycryptodome.org/)