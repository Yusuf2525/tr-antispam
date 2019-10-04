
const Discord = require('discord.js');
const antispam = require('better-discord-antispam');
const client = new Discord.Client();

antispam(client, {
        limitUntilWarn: 3,
        limitUntilMuted: 5,
        interval: 2000,
        warningMessage: "",
        muteMessage: "",
        maxDuplicatesWarning: 7,
        maxDuplicatesMute: 10,
        ignoredRoles: [],
        ignoredMembers: [],
		mutedRole:"",
		timeMuted: 1000*600,
		logChannel: ""
      });
