# Chatbox Club Blacklist
The purpose of this repo is to collect World IDs and World Names of VRChat worlds where it would not be good etiquette to display a "Now Playing" chatbox message. Club worlds or other worlds where the primary purpose is to experience a Live DJ or share in experiencing a performance of some kind.

Currently, it is hosted here on GitHub, and goes only off of worlds that have opted-in to being Blacklisted. In the future I may set up a better web API that also takes into consideration the world's tags. This is primarily an initial approach to attempt to help the situation and create relationships between OSC script developers and event runners.

## For Club Owners / Event Runners
Feel free to submit your club world to this list by either:
* If comfortable, edit the [Blacklist file](https://github.com/cyberkitsune/chatbox-club-blacklist/blob/master/npblacklist.json) here on Github and create a pull request.
* Creating a [Github Issue](https://github.com/cyberkitsune/chatbox-club-blacklist/issues/new/choose) to have the world added, if you do not wish to create a pull request.
* Contact CyberKitsune on Discord so I can add the world on your behalf, using my #club-blacklist channel on my OSC Projects Server: [Invite Link](https://discord.gg/QhTpc8Zz)

## For OSC Chatbox Script Developers
Please implement (or at least add the option) of utilizing the blacklist. I made it exposed in a simple JSON format, so it should be supported cross language and still will be supported with a similar response format if we switch to an API approach.
You should be able to fetch the latest raw blacklist file with [this URL](https://github.com/cyberkitsune/chatbox-club-blacklist/raw/master/npblacklist.json) -- the format is roughly as follows:
```json
{
  "updated": 0, // Always 0 for git
  "source": "git", // Always git for git
  "worlds": [
    {"id": "wrld_worldid-goes-here", "name": "User friendly name of world", "comment": "Comment for internal reasons (can be ignored by client)" },
  ]
}
```

If you have any suggestions, questions, or other thoughts feel free to discuss on my [Discord](https://discord.gg/QhTpc8Zz) as well!
