## Dockerfile 指令

- Dockerfile 的指令每执行一次都会在 docker 上新建一层，尽量合并同种类型的指令，通过\换行，同时让指令可读性增强。

- 全局作用

  - ENV
    - 环境变量
    - 键值对
  - LABEL
    - 为镜像添加便于管理的标志
    - 键值对

- docker build 阶段

  - FROM
    - 镜像基于的基础镜像
    - 使用官方镜像(Alpine image)
  - ARG
    - 仅 build 阶段有效的环境变量
  - WOKDIR
    - 指定工作目录
    - 推荐使用绝对路径
  - COPY
    - 复制文件/目录
    - 加 `--chown` 可更改用户和组
  - ADD
    - 类似 COPY，官方推荐 COPY
    - 区别在于 ADD 会为压缩包解压复制到目标路径，但会造成构建缓慢
  - RUN
    - 紧跟 FROM 执行命令，在 build 阶段执行
    - shell 格式，&&，pipeline
    - exec 格式: ["xxx", "xxx", "xxx"]
  - ONBUILD
    - 延迟构建命令
    - 新镜像 `from oldImage` 会执行 ONBUILD

- docker run 阶段
  - CMD
    - 运行程序，在 run 阶段执行
    - 仅最后一个生效，且 docker run 后的命令参数可以覆盖
    - 推荐格式：CMD ["可执行文件或命令", "param", ...]
  - ENTRYPOINT
    - 配合 CMD，ENTRYPOINT 为定参，CMD 传递变参
    - 仅最后一个生效，指定--entrypoint 亦可覆盖
  - VOLUME
    - 定义匿名数据卷，未指定时挂载容器
    - -v 覆盖
  - EXPOSE
    - 仅声明端口，即推荐的使用端口（express 3000， mongodb：27017）
    - 在 run 阶段使用-P，随机端口映射时会用此端口
  - USER
    - 指定后续执行指令的用户和用户组
  - HEALTHCHECK
    - 指定程序或指令监控容器服务的运行状态

## docker 的端口映射

- -P 随机映射
  - EXPOSE
- -p 指定端口
  - IP:HOST_PORT:CONTAINER_PORT
  - 宿主机端口缺失，即映射到指定地址的任意端口
  - IP 未指定，将容器的指定端口映射到宿主机的一个端口，映射所有接口地址
