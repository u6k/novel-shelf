リリース手順
============

TODO: 手動作業でのリリースとなっているので、1コマンドでリリースできるようにする。

```
cd /mnt/data/opt/novel-shelf/novel-shelf.git/
git pull origin master
cd novel-shelf-server
mvn clean package
cd ../../
cp novel-shelf.git/novel-shelf-server/target/novel-shelf-server-x.x.x.jar packages/
ln -s /packages/novel-shelf-server-x.x.x.jar novel-shelf-server.jar
```
