## Configuring SSH for Github for Windows

In GitBash:
```shell
ssh-keygen -t ed25519 -C "comment to allow you to manage keys"
```

### Configure SSH Agent with key
In Gitbash:
```shell
eval "$(ssh-agent -s)"

# add key to agent:
ssh-add <private key path>
```

### Check connection
```shell
ssh -T git@github.com
```