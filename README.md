# Big-React

从零实现 React v18 的核心功能，特点如下：

- 👬 与 React 源码最接近的极简实现
- 💪 虽然实现极简，但功能完备，当前可跑通官方测试用例数量：25
- 🚶 按`Git Tag`划分迭代步骤，记录从 0 实现的每个功能

如果想加入项目对应的`源码交流群`，和7000+小伙伴们一起交流`React`，可以加我微信，备注「开发」：

<img width="200" src="https://user-images.githubusercontent.com/15828041/181666959-57941b01-61b3-47db-9d73-ecc9ae175112.png" alt="卡颂的微信" />

## TODO List

### 工程类需求

| 类型 | 内容                               | 完成情况 | 在哪个版本实现的                                  |
| ---- | ---------------------------------- | -------- | ------------------------------------------------- |
| 架构 | monorepo（pnpm 实现）              | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| 规范 | eslint                             | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| 规范 | prettier                           | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| 规范 | commitlint + husky                 | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| 规范 | lint-staged                        | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| 规范 | tsc                                | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| 测试 | jest 环境搭建                      | ✅       | [v4](https://github.com/BetaSu/big-react/tree/v4) |
| 规范 | tsc                                | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| 构建 | babel 配置                         | ✅       | [v4](https://github.com/BetaSu/big-react/tree/v4) |
| 构建 | Dev 环境包的构建                   | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| 构建 | Prod 环境包的构建                  | ⬜️      |                                                   |
| 部署 | Github Action 执行 lint 与 test    | ⬜️      |                                                   |
| 部署 | Github Action 根据 tag 发布 npm 包 | ⬜️      |                                                   |

### 框架需求

当前跑通 React 官方测试用例 17 个

| 类型       | 内容                                   | 完成情况 | 在哪个版本实现的                                  |
| ---------- | -------------------------------------- | -------- | ------------------------------------------------- |
| React      | JSX 转换                               | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| React      | React.isValidElement                   | ✅       | [v4](https://github.com/BetaSu/big-react/tree/v4) |
| ReactDOM   | 浏览器环境 DOM 的插入                  | ✅       | [v2](https://github.com/BetaSu/big-react/tree/v2) |
| ReactDOM   | 浏览器环境 DOM 的移动                  | ✅       | [v7](https://github.com/BetaSu/big-react/tree/v7) |
| ReactDOM   | 浏览器环境 DOM 的属性变化              | ⬜️      |                                                   |
| ReactDOM   | 浏览器环境 DOM 的删除                  | ✅       | [v5](https://github.com/BetaSu/big-react/tree/v5) |
| ReactDOM   | ReactTestUtils                         | ✅       | [v4](https://github.com/BetaSu/big-react/tree/v4) |
| ReactNoop  | ReactNoop Renderer                     | ⬜️      |                                                   |
| Reconciler | Fiber 架构                             | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| Reconciler | 事件模型                               | ✅       | [v6](https://github.com/BetaSu/big-react/tree/v6) |
| Reconciler | onClick 事件支持                       | ✅       | [v6](https://github.com/BetaSu/big-react/tree/v6) |
| Reconciler | input 元素 onChange 事件支持           | ⬜️      |                                                   |
| Reconciler | Lane 模型                              | ✅       | [v8](https://github.com/BetaSu/big-react/tree/v8) |
| Reconciler | 基础 Update 机制                       | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| Reconciler | 带优先级的 Update 机制                 | ✅       | [v8](https://github.com/BetaSu/big-react/tree/v8) |
| Reconciler | 插入单节点的 mount 流程                | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| Reconciler | 插入多节点的 mount 流程                | ✅       | [v7](https://github.com/BetaSu/big-react/tree/v7) |
| Reconciler | 插入单节点的 reconcile 流程            | ✅       | [v5](https://github.com/BetaSu/big-react/tree/v5) |
| Reconciler | 插入多节点的 reconcile 流程            | ✅       | [v7](https://github.com/BetaSu/big-react/tree/v7) |
| Reconciler | 删除节点的 reconcile 流程              | ✅       | [v5](https://github.com/BetaSu/big-react/tree/v5) |
| Reconciler | HostText 类型支持                      | ✅       | [v2](https://github.com/BetaSu/big-react/tree/v2) |
| Reconciler | HostComponent 类型支持                 | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| Reconciler | HostRoot 类型支持                      | ✅       | [v1](https://github.com/BetaSu/big-react/tree/v1) |
| Reconciler | FunctionComponent 类型支持             | ✅       | [v3](https://github.com/BetaSu/big-react/tree/v3) |
| React      | Hooks 架构 mount 时实现                | ✅       | [v3](https://github.com/BetaSu/big-react/tree/v3) |
| React      | Hooks 架构 update 时实现               | ✅       | [v5](https://github.com/BetaSu/big-react/tree/v5) |
| Reconciler | useState 实现                          | ✅       | [v3](https://github.com/BetaSu/big-react/tree/v3) |
| Reconciler | useEffect 实现                         | ⬜️      |                                                   |
| Reconciler | useRef 实现                            | ⬜️      |                                                   |
| Reconciler | Legacy 调度流程（包含 batchedUpdates） | ✅       | [v8](https://github.com/BetaSu/big-react/tree/v8) |
| Reconciler | Concurrent 调度流程                    | ⬜️      |                                                   |
| Reconciler | 异常处理流程                           | ⬜️      |                                                   |
| Reconciler | useErrorBoundary 实现                  | ⬜️      |                                                   |

## 调试

提供 3 种调试方式：

1. 实时调试

执行`pnpm demo`会运行项目`demos`目录下的示例项目（默认项目是针对[v7](https://github.com/BetaSu/big-react/tree/v7)的调试项目）

这种方式的好处是：

- 控制台会打印各个主要步骤的执行信息，可以直观看到执行流程

- 热更新（包括示例代码和源码代码）

2. pnpm link

通过`CRA`或`Vite`起一个`React`测试项目后，在本项目执行`pnpm run build:dev`打包`react`与`react-dom`，在测试项目中通过`pnpm link`将项目依赖的`react`与`react-dom`替换为我们打包的`react`与`react-dom`

这种方式的好处是：最贴合项目中实际使用`React`的情况

3. 跑`React`官方的测试用例

执行`pnpm test`跑官方的测试用例，用例中引用的是执行`pnpm run build:dev`打包的`react`与`react-dom`

这种方式的好处是：可以从官方用例的角度观察框架实现的细节、各种边界情况

## 更新日志

### [v8](https://github.com/BetaSu/big-react/tree/v8)

实现了基础功能的 Lane 模型，可以调度同步更新，并基于此实现了 batchedUpdates（批处理），包括如下功能：

- Lane 模型

- 带优先级的 Update 机制

- Legacy 调度流程（包含 batchedUpdates）

- 修复了多个子节点中 number 类型节点不支持的 bug

### [v7](https://github.com/BetaSu/big-react/tree/v7)

实现了多节点 reconcile 流程（俗称的 Diff 算法），包括如下功能：

- 修复了 update 时 onClick 回调不更新的 bug

- 插入多节点的 mount 流程

- 插入多节点的 reconcile 流程

- 浏览器环境 DOM 的移动

Diff 算法的测试用例还依赖 useEffect、useRef 的实现，放在后面再实现

### [v6](https://github.com/BetaSu/big-react/tree/v6)

实现事件系统，包括如下功能：

- 事件模型
- onClick 事件支持（以及 onClickCapture 事件）

### [v5](https://github.com/BetaSu/big-react/tree/v5)

实现单节点 update，包括如下功能：

- 浏览器环境 DOM 的删除（比如 h3 变为 p，那么就要经历删除 h3、插入 p）
- 插入单节点的 reconcile 流程（包括 HostComponent、HostText）
- 删除节点的 reconcile 流程（为后续 ref、useEffect 特性做准备，实现的比较完备）
- Hooks 架构 update 时实现

### [v4](https://github.com/BetaSu/big-react/tree/v4)

初始化测试相关架构，包括如下功能：

- 实现 React.isValidElement
- jest 环境搭建
- babel 配置
- ReactTestUtils
- 跑通关于 jsx 的 17 个官方用例

### [v3](https://github.com/BetaSu/big-react/tree/v3)

实现 useState 的 mount 时流程，包括如下功能：

- FunctionComponent 类型支持
- Hooks 架构 mount 时实现
- useState 实现

### [v2](https://github.com/BetaSu/big-react/tree/v2)

插入单节点的 mount 流程（可以在浏览器环境渲染 DOM），包括如下功能：

- 浏览器环境 DOM 的插入
- HostText 类型支持

### [v1](https://github.com/BetaSu/big-react/tree/v1)

插入单节点的 render 阶段 mount 流程，包括如下功能：

- JSX 转换
- Fiber 架构
- 插入单节点的 reconcile 流程
- HostComponent 类型支持
- HostRoot 类型支持

注：还未实现浏览器环境下的渲染
