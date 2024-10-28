> 更多信息请查阅[源仓库](https://github.com/wukongdaily/DockerTarBuilder)
> 此`fork`只是定制`integration.yml`将多份架构合并于一个`actions`工作中

## 操作
### Pull and Save Docker Image 

- unzip docker-images-tar-xxx-xxxxx.zip `压缩包里不带目录，解压会将所有tar包放置当前目录中`
- 单个导入
```sh
docker load -i xxx.tar
```
- 批量导入
```sh
for file in *.tar; do
  docker load -i "$file"
done
```
