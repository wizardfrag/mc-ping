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