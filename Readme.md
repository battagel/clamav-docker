Client server setup using ClamAV daemon.

Run the docker compose to setup. This will also mount a test malware directory.

```
docker compose up --build
```

Log into the client container to emulate malware scan from client.

Run this command to scan a file or folder.

```
clamdscan <file/folder>
```
