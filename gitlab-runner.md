## IF runner is not connected try followings

```
gitlab-runner --debug run
```
or
```
gitlab-runner verfiy
```

## If getting this error failed to dial gRPC: cannot connect to the Docker daemon. Is 'docker daemon' running on this host?: dial unix /var/run/docker.sock: connect: no such file or directory
```
[[runners]]
  name = "ec2-dockerrunner-csp"
  url = "https://gitlab.com"
  id = 33475611
  token = "glrt---B-zHmq6AwL6zz2yc1k"
  token_obtained_at = 2024-03-07T09:09:51Z
  token_expires_at = 0001-01-01T00:00:00Z
  executor = "docker"
  [runners.cache]
    MaxUploadedArchiveSize = 0
  [runners.docker]
    tls_verify = false
    image = "alpine:3.15.1"
    privileged = true
    disable_entrypoint_overwrite = false
    oom_kill_disable = false
    disable_cache = false
    volumes = ["/var/run/docker.sock:/var/run/docker.sock", "/cache"]
    shm_size = 0
    network_mtu = 0

```
