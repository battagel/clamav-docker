#Client server architecture using ClamAV daemon.

## Work in Progress

- Error when connecting to latest virus db
- No remote command running e.g. API

## Setup

Run the docker compose to setup. This will also mount a test malware directory.

```
docker compose up --build
```

Log into the client container to emulate malware scan from client.

Run this command to scan a file or folder.

```
clamdscan <file/folder>
```

The logs of the file scan can be found on the **server** at:

```
/var/logs/clamav/clamd.log
```
