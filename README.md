# Viso free TV playlist

One playlist of live TV channels from around the world that broadcasters and free streaming platforms offer at no charge. Viso, the TV launcher by Miso Solutions, sets it up in the IPTV player it installs, so live TV works the first time the player opens.

## The file

`free-tv-world.m3u` is a standard M3U playlist, grouped by country. Any IPTV player can read it from:

    https://raw.githubusercontent.com/Miso-Solutions/Playlists_Viso/main/free-tv-world.m3u

`free-tv-summary.json` holds the numbers of the last build: how many streams the sources listed, how many were left out and why, how many answered, and the count per country.

## How it is built

The list is rebuilt from two public sources, [Free-TV/IPTV](https://github.com/Free-TV/IPTV) and the [iptv-org](https://github.com/iptv-org) database. Every stream has to pass the same test before it is kept:

- The stream comes from the channel's own site, from a free streaming platform's own servers, or from a server that carries only that broadcaster's channels.
- Servers that carry many unrelated channels are left out, and so are pay channels found away from their own site, adult channels and closed channels.
- Page links such as YouTube are left out, because a TV player cannot open them.
- The stream answered with a playlist or media when the list was built.

## What to expect

- A channel that answered on the build day can stop answering later. The list is rebuilt to clear those out.
- Some channels only play in their own country.
- There is no programme guide.

To report an entry that is dead or does not belong here, open an issue in this repository.
