![https://i.imgur.com/MX1Z1ys.png](https://i.imgur.com/MX1Z1ys.png)
# [NMRiH] NoBump
This plugin seeks to stop survivors constantly bumping into each other during gameplay.
It does so by rendering all teammates positioned within a set radius, referred to as the “comfort zone”, invisible to the player. This tricks said player into not soft-colliding with them. The downside to this is that all trespassing survivor models disappear for a brief moment (but only for that one player!). No other gameplay elements are affected.

##### Demo:
https://gfycat.com/FrightenedNewHarborporpoise

Keep in mind that these comfort zones do not account for client prediction. Smaller radii result in less invisibility time but prove less effective at higher latencies. By default, teammates become invisible to the player when 64 or less units away, I wouldn't recommend going under this value. 

##### Clientprefs:
Users are able to resize their comfort zone to a size that works best for them. They can also choose to disable it entirely or hide teammates at all times. This is achieved by going into **Settings** (`/settings`) > **NoBump Preferences** or with the command `/nobump`:

![https://i.imgur.com/c3mHjeB.jpg](https://i.imgur.com/c3mHjeB.jpg) 

##### Known Issues:
- Players can still bump into connecting players during practice mode.

##### Planned:
- Multilanguage support
- A beam to preview changes to a player's bubble
- Spawn dummy models instead of vanishing players entirely

##### ConVars:
- `sm_nobump_enable`(1/0) (Default: `1`)
   - Enables or disables the plugin
- `sm_nobump_default_comfort_radius` (Default: `64`)
    - By default, teammates become invisible to the player this many units away
    - Special values: `0` = Players are never hidden; `-1` = Players are always hidden

