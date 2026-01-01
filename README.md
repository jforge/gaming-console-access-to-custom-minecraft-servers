# How-to configure gaming console for use with custome minecraft servers

This repository provides some short guidelines to deal with limited capabilities of gaming consoles
to access custom minecraft servers.


## Prerequisites, Platforms and Minecraft editions

The configuration steps might differ in detail between the consoles, but the basic requirements are the same.

### Required Microsoft Account settings

You need a regular Microsoft Account and buy Minecraft accordingly.

To allow access to multiplayer games (on a dedicated server), follow the procedure in the account settings

- Step 1: Check Your Microsoft Account Settings (Essential)
- Go to Xbox Profile: Open a web browser and sign in to your Microsoft account at xbox.com.
- Navigate to Privacy: Click your profile icon (top right) > Xbox profile > Settings > Safety & privacy > Manage safety & privacy settings.
- Adjust Online Safety: Select the Xbox and Windows 10 Online Safety tab.
- Allow Multiplayer: Find "You can join multiplayer games" and set it to Allow, then click Submit.
- Restart Game: Close and relaunch Minecraft for these changes to take effect (sometimes it takes a few minutes). 


### Cross-Platform Play (Java and Bedrock)

Minecraft has two main versions: Java Edition (PC, macOS, Linux) and Bedrock Edition (iOS, Android, consoles, Windows 10/11). 

Direct connection between Java and Bedrock is not natively possible because they use different protocols.

To enable cross-play, the Java server owner must install a third-party plugin called [Geyser MC](https://geysermc.org/) 
(and optionally Floodgate plus ideally ViaVersion to overcome versioning issues when accessing an older server).
This plugin acts as a translator, allowing Bedrock clients (like your iPhone) to connect to Java servers seamlessly. 

Normally a player does not need to do anything, but might need to accept certain limitations in gameplay or server features.


### Smartphones (iOS, Android)

The Bedrock client on Smartphones allow configuration of an custom minecraft server, when selecting the "Multiplayer" option.
Add the server address and start over.

This was tested on Android with Samsumg Galaxy S2x. Please report an issue, if you face a specific issue and let's improve the guidelines.

### Nintendo Switch

When selecting the Multiplayer menu in the Minecraft client, there are only pre-configured servers available and no option to 
add another server. 

In order to still do this with your multiplayer-enabled Minecraft Account, you need to do the following:

- Change the Nintendo Switch console Primary DNS settings
- Restart the console and start Minecraft (and verify the DNS settings to be changed)
- Hit the Multiplayer button and select one of the available pre-configured server providing an "Open server list".
- This will be redirected to a page, where you can add a custom server (by IP or Domainname).
- Join the server as a Bedrock player.

#### Changing the DNS settings

You might see Primary and Secondary DNS settings like 8.8.8.8 and 1.1.1.1 in your settings.
Change the primary DNS to a server mentioned in [BedrockConnect](https://github.com/Pugmatt/BedrockConnect).

I'm using the ZAP Hosting server: 134.255.231.119 (Location: DE)
But you might be also successful with the more powerful environment with: 104.238.130.180 (Location: US).


### Microsoft XBox

For the Xbox the DNS-based approach like for the Nintendo Switch console is not possible by default. You can change the XBox primary DNS server,
but Microsoft unfortunately makes (very) sure, that this don't work; I'm not speculating about the real reasons.
Technically, this might be due to Xbox IPv6 preferences, but this was not tested and I'm not willing to disable IPv6 on my router (which would enforce IPv4).

In order to still access a custom server, you need to buy a Minecraft Realm (for € 3,99 at the time of writing), and configure it there.

The guidelines for this will follow here.


### Sony Playstation

This was not tested so far (no playstation available), AFAIK a similar approach like for the Nintendo Switch is possible.


### Others

Please report an issue, if another console should be added here.



## References

- [Minecraft](https://www.minecraft.net)
- [Minecraft Java Edition](https://minecraft.wiki/w/Java_Edition)
- [Minecraft Bedrock Edition](https://minecraft.wiki/w/Bedrock_Edition)
- [Geyser MC](https://geysermc.org/)
- [BedrockConnect](https://github.com/Pugmatt/BedrockConnect)

