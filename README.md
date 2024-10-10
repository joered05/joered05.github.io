# KeepRunningJson
This is just a place for some real-time data, such as who has experimental features enabled and if there are any in-game announcements we need to quickly send out.

Feel free to take a peak at exactly what data is received in-game: [joered05.github.io/KeepRunning/KeepRunning.json](https://joered05.github.io/KeepRunning/KeepRunning.json)

- **apiVersion:** the internal version of the API, mostly used to ensure we don't attempt to parse something and get an error.
- **experimentalFeatures**
  - **players:** just a long list of all displayNames who have enabled experimental features.
    - *long list of player display names...*
  - **killSwitch:** a simple switch we can flip if a game-breaking bug is discovered with an experimental feature. This is significantly quicker and easier than an entire game update.
- **attentionBoard:** a message we can put in-game if we need to quickly announce something in-game, such as if a recent VRChat update breaks some feature. Just like the killSwitch above, this can be sent much quicker than a game update.
- **communityMonsterImage:** data about the current and legacy community monster images. This allows us to change it without needing to push a game update.
  - **author:** the author of the [current community monster image](https://joered05.github.io/KeepRunning/CurrentCommunityMonsterImage.png) (current *audio* [here](https://joered05.github.io/KeepRunning/CurrentCommunityMonsterAudio.mp4))
  - **legacy:** data specifically for legacy images.
    - **height:** the height and width of the legacy community monster image, [viewable here.](https://joered05.github.io/KeepRunning/LegacyCommunityMonsterImages.png)
    - **pixelsPerMonster:** the amount of pixels each monster takes up.
    - **authors:** A list of all the previous community monsters images authors, in order of how they appear on the [legacy community monster image](https://joered05.github.io/KeepRunning/LegacyCommunityMonsterImages.png), starting from top left.
      - *long list of player display names...*
