# Jupyter

- [Installing Jupyter Software](https://jupyter.org/install)
- [Jupyter Server](https://jupyter-server.readthedocs.io/en/latest/index.html)

## 配置

1. 生成配置文件

```shell
jupyter notebook --generate-config
jupyter server --generate-config
```

2. 修改配置文件

```shell
c.ServerApp.root_dir = <root dir>
c.ServerApp.use_redirect_file = False # WSL environment
```

3. 设置密码

```shell
jupyter notebook password
```

4. 后台运行

```shell
nohup jupyter notebook >/dev/null 2>~/jupyterlab.err &
```

## lineWrap

Settings -> Advanced Settings Editor -> Notebook to user preferences add:

```json
{
    "codeCellConfig": {
        "lineWrap": "on"
    }
}
```
