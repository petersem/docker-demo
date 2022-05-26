# Synology All-In-One - a demo of a few different containers
This will install and create containers for the following apps
- Plex
- Posterr
- Watchtower
- Dozzle
- Autoheal
- Radarr
- Sonarr
- Lidarr
- Readarr
- Prowlarr
- Bazarr
- Sabnzbd
- Qbittorrent
> Do not use Qbittorrent until it is protected by a VPN

## Prerequisites
- Install the docker package
- Best with OpenVPN/Wireguard/Another VPN? (Needed for Qbittorrent)

### Folders
The following folders should be created. You can copy/paste these into a terminal
- cd /volume1/downloads/complete
- cd /volume1/downloads/incomplete
- cd /volume1/docker/prowlarr
- cd /volume1/docker/sonarr
- cd /volume1/docker/radarr
- cd /volume1/docker/lidarr
- cd /volume1/docker/bazarr
- cd /volume1/docker/readarr
- cd /volume1/docker/sabnzbd
- cd /volume1/docker/plex
- cd /volume1/docker/plex/transcode
- cd /volume1/docker/plex/config
- cd /volume1/docker/portainer
- cd /volume1/docker/tautulli
- cd /volume1/docker/posterr
- cd /volume1/docker/poster/config
- cd /volume1/docker/poster/randomthemes
- cd /volume1/docker/gaps

Your media path should be one top-level folder with sub folders for different media types 
> For example:
> - media
>   - movies
>   - tv
>   - music
>   - ebooks

### Changes to .env file
Review the .env and update
- TZ
- PUID
- PGID
- Path values
- plex-specific values
