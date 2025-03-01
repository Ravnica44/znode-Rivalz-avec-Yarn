Check if you have a license before starting this tutorial at https://znode.rivalz.ai/licenses

https://docs.rivalz.ai/znode-validators/running-a-znode

```shell
adduser znode
```

```shell
sudo usermod -aG sudo znode
```
```shell
screen -S Znode
```

```shell
su - znode
```

```shell
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
```

```shell
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
```

```shell
sudo apt update
```

```shell
sudo apt install -y nodejs
```

```shell
sudo apt install --no-install-recommends -y yarn
```


```shell
echo 'export PATH="$(yarn global bin):$PATH"' >> ~/.bashrc
source ~/.bashrc
```

```shell
yarn --version
```

```shell
yarn global add rivalz-znode-cli@latest
```

```shell
echo 'export PATH="$PATH:/home/rivalz/.yarn/bin"' >> ~/.bashrc && source ~/.bashrc
```

```shell
znode run
```

For new zNodes, without licenses inside
If you are trying to run a zNode without any license yet, to check the delegate code and you got an error, use this command instead
`znode info`

After that you can use the delegate code from the program in our zNode Panel to make the delegation.
When delegation is done, you can return to the program and run the zNode with
`znode run`
