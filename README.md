# Interlock + HAProxy + Swarm + Machine

[Interlock](https://github.com/ehazlett/interlock) configured to use HAProxy and a Swarm that has been set up with Machine.

Use it by configuring your shell to point at your Swarm master, then run this image on it:

```
$ eval "$(docker-machine env --swarm swarm-master)"
$ docker run -e DOCKER_HOST -v /etc/docker:/etc/docker bfirsh/interlock-haproxy-swarm
```

