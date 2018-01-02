# What is ElectroneumD?

ElectroneumD is the console full node & miner provided by [electroneum](https://github.com/electroneum/electroneum).

ElectroneumD supports Electroneum (ETN).

# How to use this image [X86_64 version]

Create shared volume:

```console
$ docker volume create --name electroneumd
```

Run in background:

```console
$ docker run -v electroneumd:/electroneumd -d --name YOUR_CONTAINER_NAME -p YOUR_PORT_1-YOUR_PORT_3:YOUR_PORT_1-YOUR_PORT_3 calvintam236/electroneumd:x86_64 --non-interactive --data-dir /electroneumd --no-igd --rpc-bind-port YOUR_PORT_1 --rpc-bind-ip 0.0.0.0 --rpc-login YOUR_DAEMON_USERNAME:YOUR_DAEMON_PASSWORD --confirm-external-bind
```

Get `electroneumd` options with:

```console
$ docker run --rm calvintam236/electroneumd:x86_64
```

Fetch logs of a container:

```console
$ docker logs YOUR_CONTAINER_NAME
```
