# Egg-server-docker



## QuickStart

<!-- add docs here for user -->

see [egg docs][egg] for more detail.

### Development
```shell
$ docker-compose up
```

### Deploy

Use `EGG_SERVER_ENV=docker` to test

Use `EGG_SERVER_ENV=prod` to prod

### Dependence

Daocloud docker engine

### Update

git subtree:

* http://blog.zlxstar.me/blog/2014/07/18/git-submodule-vs-git-subtree/
* https://gist.github.com/kvnsmth/4688345

```
git remote add origin https://github.com/giftman/egg-server-docker.git
git push -u origin master

git subtree split --prefix=src --branch egg-server

#push to egg-server
git push https://github.com/giftman/egg-server-docker.git egg-server:master

#pull to update 
git subtree pull --prefix=src --squash https://github.com/giftman/egg-server.git master
```

I pull to update fail,I don't know why, solve next time..