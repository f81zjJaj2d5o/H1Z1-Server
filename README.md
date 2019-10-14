# H1Z1-Server

## What is this project?

This project aim to make a server for the December 22 2016 version of H1Z1 (Survival Aspect).

**How to use?**

Just compile the project via Visual Studio and start the server, by default it starts on `localhost:20042`.
Open your game folder then edit the `ClientConfig.ini` file at the second line and set the LoginServer IP & Port.
Copy the `Launcher.exe` file from the git repo and paste it into the game folder, you will have to use this launcher to start the game.

You can also download the 2016 version of the game via steam if you bought H1Z1 by typing `download_depot 295110 295111 8395659676467739522` in the steam console.

## State

- [ ] Login server
- [ ] Gateway server
- [ ] Zone server

## Info for devs

The login server handle the client session request and reply to it, then it sends the gateway server ip/port. The gateway server sends the zone servers list that are shown in the lobby and finally, when the client connect to a server from the list it connects to the zone server and perform request about the map/player packets...

## Credits

[loguru](https://github.com/emilk/loguru) - for the log utility

[cpp-httplib](https://github.com/) - for the http server

[rapidjson](https://github.com/) - for the json utility
