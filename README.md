# FFAI: Fantasy Football AI
FFAI is a python package that includes a framework for playing and developing bots for digital fantasy-football board-games.
For an in-depth description of the framework, challenge of applying AI to fantasy football, and some preliminaray results see our paper: [A New Board Game Challenge and Competition for AI](https://njustesen.files.wordpress.com/2019/07/justesen2019blood.pdf).

![FFAI](docs/screenshots/ffai.png?raw=true "FFAI")

Please cite our paper if you use FFAI in your publications.
```
@inproceedings{justesen2019blood,
  title={Blood Bowl: A New Board Game Challenge and Competition for AI},
  author={Justesen, Niels and Moore, Peter David and Uth, Lasse M{\o}ller and Togelius, Julian and Jakobsen, Christopher and Risi, Sebastian}
  booktitle={2019 IEEE Conference on Games (COG)},
  year={2019},
  organization={IEEE}
}
```

## Plans for Future Releases
* Support for all skills and teams in LRB6 + BB2016
* AI interface using protobufs to enable any programming language
* Integration with OBBLM/NAFLM
* Support for dungeon arenas

## Installation
[Make sure python 3.6 or newer is installed, together with pip.](https://www.makeuseof.com/tag/install-pip-for-python/)
Then run:
```
pip install git+https://github.com/njustesen/ffai
```

## Run FFAI's Web Server
```
python -c "import ffai.web.server as server;server.start_server(debug=True, use_reloader=False, port=5000)"
```
Or download the examples folder and run:
```
python examples/server_example.py
```
Go to: http://127.0.0.1:5000/

The main page lists active games. For each active game you can click on a team to play it. If a team is disabled it is controlled by a bot and cannot be selected. Click hot-seat to play human vs. human on the same machine.

## Disclaminers and Copyrighted Art
FFAI is not affiliated with or endorsed by any company and/or trademark. FFAI is an open research framework and the authors have no commercial interests in this project. The web interface in FFAI currently uses a small set of icons from the Fantasy Football Client. These icons are not included in the license of FFAI. If you are the author of these icons and don't want us to use them in this project, please contact us at njustesen at gmail dot com, and we will replace them ASAP. The team icons are from FUMBBL and are used with permission. The license described in [LICENSE](LICENSE) only covers the source code - not any of the graphics files.

## Get Involved
Do you want implement a bot for FFAI or perhaps help us test, develop, and/or organize AI competitions? Join the [FFAI Discord server](https://discord.gg/MTXMuae).
