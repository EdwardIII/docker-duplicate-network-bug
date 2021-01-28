To replicate:

./hook


You should see an error like:

```
Error response from daemon: network duplicate-network_default is ambiguous (2 matches found on name)
Looks like you forgot to fix a linting issue on busybox
Creating network "duplicate-network_default" with the default driver
Creating duplicate-network_busybox_run ... done
Error response from daemon: network duplicate-network_default is ambiguous (2 matches found on name)
```

And networks like this:

```
NETWORK ID     NAME                        DRIVER    SCOPE
f2daada15deb   bridge                      bridge    local
614a5859223f   duplicate-network_default   bridge    local
b5458442575f   duplicate-network_default   bridge    local
```
