
### 前端启动：  
1.安装对应的版本node ： [下载地址](https://nodejs.org/dist/latest-v12.x/)
2.安装到用户node版本下
```shell 
vim ~/.bash_profile 
export NODEROOT="/User/node/current"
export PATH=$PATH:$NODEROOT/bin

```

确认版本：
```shell 
node -v 
```

安装 yarn 
```shell 
npm install -g yarn 
```

安装

```shell
npm install -g node-gyp
```



3.安装依赖  

```shell 
对应的项目路径下执行 ： 
yarn install --pure-lockfile 
```
4. 启动前端 
```shell 
yarn start 
```
### 后端编译 
配置好对应的GOROOT，GOPATH

grafana 需要注意GOPATH 下src/github.com/grafana/grafana 才是代码。  
```shell
编译： 
go run build.go build 
```

### 启动脚本： 
```shell
grafana-server --homepath=/Users/caihaisong/Code/Github/grafanaCodeStable/src/github.com/grafana/grafana --config=/Users/caihaisong/Code/Github/grafanaCodeStable/src/github.com/grafana/grafana/conf/defaults.ini cfg:default.log.mode=console cfg:default.paths.data=/Users/caihaisong/Code/Github/grafanaCodeStable/src/github.com/grafana/grafana/data cfg:default.paths.logs=/Users/caihaisong/Code/Github/grafanaCodeStable/src/github.com/grafana/grafana/log cfg:default.paths.plugins=/Users/caihaisong/Code/Github/grafanaCodeStable/src/github.com/grafana/grafana/plugins cfg:default.paths.provisioning=/Users/caihaisong/Code/Github/grafanaCodeStable/src/github.com/grafana/grafana/conf/provisioning
```