# lrew git-sync

监听 git 变化，并克隆到本地。

* https://packagist.org/packages/lrew/
* https://docs.lnmp.khs1994.com/lrew.html

* https://github.com/kubernetes/git-sync

## 用法

`docker-compose`

```yaml
...

php7:
  volumes:
  - git-sync-data:/app/git-sync

nginx:
  volumes:
  - git-sync-data:/app/git-sync
```

nginx `www.conf`

```nginx
server {
  ...
  root /app/git-sync/git-sync;
}
```
