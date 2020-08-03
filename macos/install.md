# MacOS Install

## Contents

 - [Install Redis](#install_redis)

## <a name="install_redis"></a>Install Redis

Redis could be installed from `brew`.

```shell
brew install redis
```

Then the service should be started:

```shell
brew services start redis
```

Then test if the service is ready:

```shell
redis-cli ping
```
