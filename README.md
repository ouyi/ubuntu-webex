# About

Dockerized Cisco WebEx based on 32-bit Ubuntu. Desktop sharing works (tested on Fedora 23).

# Known issues

Personal rooms not supported according to https://help.webex.com/docs/DOC-4748

# Run

xhost localhost:$(whoami)
docker run --rm -ti -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=unix$DISPLAY ouyi/ubuntu-webex