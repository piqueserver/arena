# About

> Pre-configured arena setup for piqueserver

# Usage

```bash
git clone https://github.com/piqueserver/arena && cd arena
vim config.toml # edit servername/passwords/enable irc relay etc.
piqueserver -d . # note: requires master version i.e. you'll have to install from source
# or, with docker/docker-compose
docker-compose up -d # note: -d here, daemonizes it
docker-compose down  # shutting it down
```

# Config directory

Structure as follows:

```
.
├── config.toml                 # default config file if no file specified on command line
├── logs                        # logs directory
│   └── log.txt                 #  default server logfile
├── maps                        # maps in .txt generate script form or .vxl data
│   ├── classicgen.txt          #  includes a couple of simple maps - add any maps you want to use here
│   └── ...
└── scripts                     #  Scripts inside this directory get loaded. 
    ├── __init__.py             #  don't delete this - needed so python can import scripts for this directory
    ├── my_custom_script.py     #  Note: pique already includes commonly used scripts
    └── ...
```

# Map Credits

Maps in this repo. belong to their respective creator.

```
cs_assault - Danke-o
cs_havana  - Danke-o
csitaly    - Danke
csoffice   - Danke
de_aztec   - Danke
de_dust    - Danke-o
de_train   - Megastar
```