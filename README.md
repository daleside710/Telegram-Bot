Introduction
This library provides a pure Python interface for the Telegram Bot API. It's compatible with Python versions 2.7, 3.3+ and PyPy.

Installing
Beta note

The newest stable release is currently version 11.1.0.

The newest release is a beta release for version 12. Install or upgrade with:

$ pip install python-telegram-bot==12.0.0b1 --upgrade
See CHANGES.rst for the changelog and make sure to report any bugs you find!

You can install or upgrade the stable python-telegram-bot with:

$ pip install python-telegram-bot --upgrade
Or you can install from source with:

$ git clone https://github.com/python-telegram-bot/python-telegram-bot --recursive
$ cd python-telegram-bot
$ python setup.py install
In case you have a previously cloned local repository already, you should initialize the added urllib3 submodule before installing with:

$ git submodule update --init --recursive

Logging
This library uses the logging module. To set up logging to standard output, put:

import logging
logging.basicConfig(level=logging.DEBUG,
                    format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
at the beginning of your script.

You can also use logs in your application by calling logging.getLogger() and setting the log level you want:

logger = logging.getLogger()
logger.setLevel(logging.INFO)
If you want DEBUG logs instead:

logger.setLevel(logging.DEBUG)