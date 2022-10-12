# WorkspaceTemplate

这是一个 pnpm 工作簿的一个模板项目

## Includes

- [x] TypeScript@4.7.4
- [x] build (Rollup@2.77)
- [x] test (vitest@0.22)

## Get started

## 1. 进入工作目录

> mkdir PackageName
> cd PackageName

## 2. 下载模板

> degit mekefly/workspace-template

## 主要功能

- pnpm
  - `script` 负责 scripts 的一些处理类 等于 `node scripts` 命令
    - `--reBuild` 重新构建命令
    - `build` 构建整个项目，工作空间终的包
      - `-v, --version` Display version number
      - `-I, --inputPath` <inputPath> 可以用,号分隔写多个 默认值：[空]
      - `-W, --workSpace` <workSpace> 可以用,号分隔写多个 默认值：[空]
      - `--includePackages` <includePackages> 可以用,号分隔写多个 默认值：
      - `--include` <include> 可以用,号分隔写多个 默认值：
      - `-P, --packages` <packages> 可以用,号分隔写多个 默认值：[空]
      - `-O, --output` <output> dist
      - `-F, --format` <format> 可以用,号分隔写多个 默认值：[空]
      - `--prod` <prod> 可以用,号分隔写多个 默认值：[空]
      - `-D, --declaration` <declaration> true
      - `--watch` <watch> false
      - `--disableConcurrent` <disableConcurrent> false
      - `-w, --watch` 监听更改
      - `-h, --help` Display this message
    - `create` 创建子项目模板
      - `--help` create 子命令的帮助
      - `<PackageName>` 子项目的名字
  - `testScript` 单元测试 scripts 脚本
  - `test` 单元测试
  - `build` 等于 `pnpm script build $` 命令
