# JAX框架笔记

## 环境安装
[JAX 官方页面](https://github.com/google/jax)



由于我所在实验室的公用GPU服务器是Windows平台+jupyter lab的环境配置，而JAX原生不支持该平台，无法安装`jaxlib`。因此在GitHub上找到["cloudhan/jax-windows-builder"](https://github.com/cloudhan/jax-windows-builder)这个项目，通过下面的语句完成`JAX`的安装。

```shell
pip install jax[cuda111] -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
```