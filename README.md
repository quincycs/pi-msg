# pi-msg

Let Pi sessions talk to each other via Unix sockets.

## Install

pi install git:github.com/m7l5/pi-msg

## Usage

/msg-on [name]       Join the msg network
/msg-off             Leave the msg network
/msg-list            List online sessions
/msg-send <name>     Send a message

## How it works

Sockets at ~/.pi/msg/<name>.sock.

Online detection = can you connect to the socket?
Offline = socket doesn't exist or refuses connection.

## Roadmap

- [ ] Incoming message notifications in TUI
- [ ] Cold-session wake-up via SDK
- [ ] Named session discovery
