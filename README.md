### Monorepo - Lerna

> 相关知识点

1. npm查看全部安装的包

```
npm list -g / npm ls -g    // 把包的所有依赖也显示出来
npm ls -g --depth 0        // 只会查到安装的包，不会查到包的依赖
```

2. npm查看当前项目已安装的包（必须有package.json文件）

```
npm list  /  npm ls    // 同上
npm ls --depth 0       // 同上
```

> package.json 配置说明
1. workspaces: ['packages/*']    // 表示工作区是packages下的所有子目录
2. private: true    // 表示项目的根目录不会被发不出去
