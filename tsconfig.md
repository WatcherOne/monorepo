### tsconfig

1. npx tsc --init     // 将创建一个 typescript 默认配置文件 (tsconfig.json)
2. compilerOptions: {
    outDir: "dist"      // 编译后输出目录, 默认编译后的文件位置将和ts源文件在同一位置
    declaration: true   // 指定是否在编译完成后生成相应的*.d.ts文件, 默认 false
}
3. 配置 package.json {
    "scripts": {
        "tsc": "tsc"    // 可以通过 npm run tsc 来编译ts文件转为js文件
    }
}
