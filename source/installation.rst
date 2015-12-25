.. _installation:

Installation
============

Installing on Windows
---------------------

You need to install PocketMine first before installing ImagicalMine on Windows. Follow the instructions below to install PocketMine and ImagicalMine.

Download the latest version from `PocketMine`_.
Use the installer to install PocketMine-MP.
The installer may have an outdated version of ImagicalMine.
You can download the latest .phar from `Jenkins`_.

.. warning::
    If the provided x64 binary does not work then try the x86 binary.

Installing on Linux/MacOS
-------------------------

Use one of the following urls depending on which "bit" operating system you have with ``curl`` or ``wget`` to install ImagicalMine directly.

.. code-block:: sh

	http://get.imagicalcorp.ml/Linux32
        http://get.imagicalcorp.ml/Linux64
        http://get.imagicalcorp.ml/Mac32
        http://get.imagicalcorp.ml/Mac64

Replace ``<URL>`` with one from above.

.. code-block:: sh

	curl -sL <URL> | bash
	wget -q -O - <URL> | bash

.. code-block:: sh

  ImagicalMine installation finished. Run ./start.sh to start ImagicalMine.


Installing on Android
---------------------

Install `PocketMine-MP for Android`_ from the Google play.

Starting for the first time
---------------------------

Now you should be able to start ImagicalMine.
The first time it starts with a set-up wizard,
this can be disabled by running ``./start.sh --no-wizard``.

.. code::

    $ ./start.sh
    [*] ImagicalMine set-up wizard
    [*] Please select a language:
    English => en
    EspaÃ±ol => es
    ä¸­æ–‡ => zh
    PyccÄ¸Ð¸Ð¹ => ru
    æ—¥æœ¬èªž => ja
    Deutsch => de
    í•œêµ­ì–´ => ko
    Nederlands => nl
    FranÃ§ais => fr
    Italiano => it
    Melayu => ms
    Norsk => no
    Svenska => sv
    Suomi => fi
    TÃ¼rkÃ§e => tr
    [?] Language (en):

ImagicalMine supports a few other languages.
Fill in the two letters behind the language and press enter.
Is your language not in the list? Add it on `Crowdin`_.

.. code::

    [*] English has been correctly selected.
    Welcome to ImagicalMine!
    Before starting setting up your new server you have to accept the license.
    ImagicalMine is licensed under the LGPL License,
    that you can read opening the LICENSE file on this folder.

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Lesser General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    [?] Do you accept the License? (y/N):

Do you accept the `License`_?

.. code::

    [?] Do you want to skip the set-up wizard? (y/N):

You can skip the wizard from here and start the server with the default settings or continue.

.. code::

    [*] You are going to set up your server now.
    [*] If you don't want to change the default value, just press Enter.
    [*] You can edit them later on the server.properties file.
    [?] Give a name to your server (Minecraft: PE Server):
    [*] Do not change the default port value if this is your first server.
    [?] Server port (19132):
    [*] The RAM is the maximum amount of memory ImagicalMine will use. A value of 128-256 MB is recommended
    [?] Server RAM in MB (256):
    [*] Choose between Creative (1) or Survival (0)
    [?] Default Game mode: (0):
    [?] Max. online players (20):
    [*] The spawn protection disallows placing/breaking blocks in the spawn zone except for OPs
    [?] Enable spawn protection? (Y/n):
    [*] An OP is the player admin of the server. OPs can run more commands than normal players
    [?] OP player name (example, your game name):
    [!] You will be able to add an OP user later using /op <player>
    [*] The white-list only allows players in it to join.
    [?] Do you want to enable the white-list? (y/N):
    [!] Query is a protocol used by different tools to get information of your server and players logged in.
    [!] If you disable it, you won't be able to use server lists.
    [?] Do you want to disable Query? (y/N):
    [*] RCON is a protocol to remote connect with the server console using a password.
    [?] Do you want to enable RCON? (y/N):
    [*] Getting your external IP and internal IP
    [!] Your external IP is x.x.x.x. You may have to port-forward to your internal IP x.x.x.x.
    [!] Be sure to check it, if you have to forward and you skip that, no external players will be able to join. [Press Enter]
    [*] You have finished the set-up wizard correctly
    [*] Check the Plugin Repository to add new features, minigames, or advanced protection to your server
    [*] ImagicalMine will now start. Type /help to view the list of available commands.

    [Server thread/INFO]: Loading imagicalmine.yml...
    [Server thread/INFO]: Loading server properties...
    [Server thread/INFO]: Selected English (eng) as the base language
    [Server thread/INFO]: Starting Minecraft: PE server version v0.11.0 alpha
    [Server thread/NOTICE]: The memory-limit setting has been deprecated.
    [Server thread/NOTICE]: There are new memory settings on pocketmine.yml to tune memory and events.
    [Server thread/NOTICE]: You can also reduce the amount of threads and chunks loaded control the memory usage.
    [Server thread/INFO]: Opening server on 0.0.0.0:19132
    [Server thread/INFO]: This server is running ImagicalMine version 1.0dev「[ImagicalMine]」(API 1.13.0)
    [Server thread/INFO]: ImagicalMine is distributed under the LGPL License
    [Server thread/INFO]: Preparing level "world"
    [Server thread/INFO]: Starting GS4 status listener
    [Server thread/INFO]: Setting query port to 19132
    [Server thread/INFO]: Query running on 0.0.0.0:19132
    [Server thread/INFO]: Default game type: Survival Mode
    [Server thread/INFO]: Done (19.485s)! For help, type "help" or "?"

The server should have started now and you should be able to join.

.. _PocketMine: https://pocketmine.net
.. _Win-Bintray: https://bintray.com/pocketmine/PocketMine/Windows-PHP-Binaries/view#files
.. _GitHub: https://github.com/ImagicalCorp/ImagicalMine/releases
.. _Jenkins: http://jenkins.pocketmine.net/job/PocketMine-MP
.. _PHP-Bintray: https://bintray.com/pocketmine/PocketMine/Unix-PHP-Binaries/view#files
.. _PHP-Jenkins: http://jenkins.pocketmine.net/
.. _PM-Stable: https://github.com/PocketMine/PocketMine-MP/releases
.. _PM-Dev: http://jenkins.pocketmine.net/job/PocketMine-MP/
.. _PocketMine-MP for Android: https://play.google.com/store/apps/details?id=net.pocketmine.server
.. _Crowdin: http://translate.pocketmine.net
.. _License: https://github.com/ImagicalCorp/ImagicalMine/blob/master/LICENSE
.. _ImagicalMine-Jenkins: http://jenkins.imagicalcorp.ml:8080/job/ImagicalMine
