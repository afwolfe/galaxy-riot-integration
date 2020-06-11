# Riot Integration - v0.1.3

Self explanatroy, a GOG Galaxy 2.0 Community integration for Riot! If you're wondering why the icon is odd (missing) see this [issue](https://github.com/urwrstkn8mare/gog-riot-integration/issues/1#issuecomment-641019594).

## Usage

It's pretty simple. Just place unzip the file from [releases](https://github.com/urwrstkn8mare/gog-riot-integration/releases) and place the folder in `%LOCALAPPDATA%\GOG.com\Galaxy\plugins\installed`. For the plugin to detect any installed Riot games, they must be in your start menu shortcuts. This is simply done by leaving the option to add a desktop shorcut checked (it's checked by default). If you don't want the desktop shortcut, you may delete it as it's not required.

Note: As of now, the path to `RiotClientServices.exe` is set by default to `C:\Riot Games\Riot Client\RiotClientServices.exe`. To change it create a file called `riot_client_location.txt` and put the path to the executable in it. Then place the file in `%LOCALAPPDATA%\GOG.com\Galaxy\plugins\installed`. ([need help?](https://youtu.be/rcwvYqD1w7Q))

## Known Issues

- ~~If you press sync integratiom games lose installed status for some reason (working on it right now!)~~

## FAQ

- _Game time doesn't show the time before I added the plugin._
  That's because Riot doesn't record gametime. The plugin will only display gametime while you've launched it via GOG Galaxy 2.0 just like if you had added it manually.

## Todo

Any help (and feedback about this project) would be appreciated! If you want to add something or do a task feel free to do it and I'd appreciate a pull request.

- [ ] Add Mac support (don't have much time for it right now)
- [ ] Automatically determine path to `RiotClientServices.exe`. (need to parse target path from Windows shortcuts. spoiler alert - it's hard)
- [ ] Not require start menu shortcuts to be available. (can't figure this out)
- [ ] Support friend recomendation and presence. (this may or may not be possible though)
- [ ] Maybe changed the formatting of the code to something other than [Black](https://github.com/psf/black). Its consistent but not as nice as some other styles of formatting.

## Credits

- Heavy inspiration from <https://github.com/FriendsOfGalaxy/galaxy-integration-minecraft>, the fork of: <https://github.com/TouwaStar/Galaxy_Plugin_Minecraft>
- <https://github.com/tylerbrawl/Galaxy-Utils>
- And of course: <https://github.com/gogcom/galaxy-integrations-python-api>

## Development / Build Release

`python3 -m pip install -r requirements.txt -t .`
