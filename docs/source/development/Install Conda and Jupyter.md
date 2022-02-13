# Install Conda and Jupyter

## Conda

- [Installing on Linux](https://docs.anaconda.com/anaconda/install/linux/)
- [Latest Miniconda Installer](https://docs.conda.io/en/latest/miniconda.html)
- [Command reference](https://docs.conda.io/projects/conda/en/latest/commands.html)
- [Updating from older versions](https://docs.anaconda.com/anaconda/install/update-version/)

## Jupyter

- [Installing Jupyter Software](https://jupyter.org/install)
- [Jupyter Server](https://jupyter-server.readthedocs.io/en/latest/index.html)

### 配置

1. 生成配置文件

```shell
jupyter notebook --generate-config
jupyter server --generate-config
```

2. 修改配置文件

修改内容：

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

### lineWrap

Settings -> Advanced Settings Editor -> Notebook to user preferences add:

```json
{
    "codeCellConfig": {
        "lineWrap": "on"
    }
}
```

## pip

- [Upgrading pip](https://pip.pypa.io/en/stable/installation/#upgrading-pip)
- [Python Package Index](https://pypi.org/)

## nodejs

- [Debian and Ubuntu based Linux distributions](https://github.com/nodesource/distributions/blob/master/README.md)
