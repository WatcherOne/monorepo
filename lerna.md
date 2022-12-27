### Lerna

1. npx lerna    // 安装 lerna (全局安装-g)
2. lerna init   // 将现有仓库升级为适配当前版本的 lerna
3. lerna create <package_name>  // 创建包项目
4. lerna bootstrap  // 在包中安装依赖
5. npm login      // 登录到 npm 上
6. lerna publish  // 将包发布到 npm 上【可能会报错没有提交到git仓库中】


> 运行命令【上述命令其实就是对如下做的封装, lerna毕竟也是工具框架】
1. yarn workspace <workspace_name> add react react-dom --dev
2. yarn add <> -D -W     //  如果某些依赖是所有package通用的则安装在根目录的依赖下即可
3. yarn workspace run serve
4. yarn workspace run build
5. yarn workspaces run build      // 对所有package中运行指定的命命, (若某个包中没有对应的命令则会报错)
6. yarn workspaces info [--json]  // 查看项目中的workspace依赖树
