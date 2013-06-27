# mc-ping

This is a super-simple library that provides access to the [Server-list-ping](http://wiki.vg/Server_List_Ping) feature of Minecraft servers.

You can use it as follows

    mcping = require('mc-ping');
    mcping('yourserver.com', 25565, function(err, res) {
    	if (err) {
    		// Some kind of error
    		console.error(err);
    	} else {
    		// Success!
    		console.log(res);
    	}
	});

In this instance, `res` will be a javascript object similar to the following:

    { protocol_version: '51',
      minecraft_version: '1.4.7',
      server_name: 'Your Server MOTD',
      num_players: '0',
      max_players: '20' }

## License

(MIT License)

Copyright (C) 2013 David White &lt;david@wizardfrag.co.uk&gt;

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.