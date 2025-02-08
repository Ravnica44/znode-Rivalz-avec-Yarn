https://docs.rivalz.ai/znode-validators/running-a-znode

```shell
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update && sudo apt install yarn
```

```shell
yarn --version
```

```shell
yarn global add rivalz-znode-cli@1.7.2
```

For new zNodes, without licenses inside
If you are trying to run a zNode without any license yet, to check the delegate code and you got an error, use this command instead
znode info

After that you can use the delegate code from the program in our zNode Panel to make the delegation.
When delegation is done, you can return to the program and run the zNode with
znode run
)
