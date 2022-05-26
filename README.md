# Synology All-In-One - a demo of a few different containers
This will install and create containers for the following apps
- Autoheal
- Bazarr
- Dozzle
- Gaps
- Lidarr
- Plex
- Portainer
- Posterr
- Prowlarr
- Qbittorrent
- Radarr
- Readarr
- Sabnzbd
- Sonarr
- Tautulli
- Watchtower
> Do not use Qbittorrent until it is protected by a VPN

## Prerequisites
- Install the docker package
- Best with OpenVPN/Wireguard/Another VPN? (Needed for Qbittorrent)
- This is configured for machines that have an Intel Quicksync GPU
  If you do not have one of these, edit the docker-compose.yaml and find the section on Plex. At the end of the section are two lines for "device:". Remove, or comment theses lines and it will all work. 

### Folders
The following folders should be created. You can copy/paste these into a terminal
- mkdir /volume1/downloads/complete
- mkdir /volume1/downloads/incomplete
- mkdir /volume1/docker/bazarr
- mkdir /volume1/docker/gaps
- mkdir /volume1/docker/lidarr
- mkdir /volume1/docker/plex
- mkdir /volume1/docker/plex/transcode
- mkdir /volume1/docker/plex/config
- mkdir /volume1/docker/portainer
- mkdir /volume1/docker/posterr
- mkdir /volume1/docker/posterr/config
- mkdir /volume1/docker/posterr/randomthemes
- mkdir /volume1/docker/prowlarr
- mkdir /volume1/docker/qbittorrent
- mkdir /volume1/docker/radarr
- mkdir /volume1/docker/readarr
- mkdir /volume1/docker/sabnzbd
- mkdir /volume1/docker/sonarr
- mkdir /volume1/docker/tautulli

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
