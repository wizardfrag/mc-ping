# mc-ping

This is a super-simple library that provides access to the [Server-list-ping](http://wiki.vg/Server_List_Ping) feature of Minecraft servers.

You can use it as follows

    mcping = require('mc-ping');

    mcping('yourserver.com', 25565, console.log);

It will return a javascript object similar to the following:

    { protocol_version: '51',
      minecraft_version: '1.4.7',
      server_name: 'Your Server Name',
      num_players: '0',
      max_players: '20' }