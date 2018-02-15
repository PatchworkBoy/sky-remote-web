# sky-remote-web

Combined http request / Web interface for sending remote control commands to a Sky TV box.

It is basic and *was* ugly, but functional.

#### Usage - Web Control

Just start the script, and then open a browser at `http://localhost:29152`.

Ensure the text box at the top of the page contains the IP address of your Sky box.

Nothing more to it.

Sky remote skin by DJBenson.

#### Usage - HTTP Request

Fire a POST or GET request to `http://localhost:29152/control/`

If using GET, append query parameters `?ip=192.168.0.16&command=pause`
If using POST, send a JSON payload `{ip: 192.168.0.16, command: 'pause'}`

Available commands are equivalent to the same button presses on the Sky Remote:
* power,
* select,
* backup,
* dismiss,
* channelup,
* channeldown,
* interactive,
* sidebar,
* help,
* services,
* search,
* tvguide,
* home,
* i,
* text,
* up,
* down,
* left,
* right,
* red,
* green,
* yellow,
* blue,
* 0,
* 1,
* 2,
* 3,
* 4,
* 5,
* 6,
* 7,
* 8,
* 9,
* play,
* pause,
* stop,
* record,
* fastforward,
* rewind,
* boxoffice,
* sky
