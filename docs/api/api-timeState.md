## API

statelink 是一个状态管理库，能够自动管理函数与其内部引用状态的关系。

### 特色

- 通过赋值更新依赖函数
- 简化组件数据流转
- 极简的状态回溯能力
- 自动计算最小依赖执行

### 安装

statelink 可单独使用，也可以配合 React Hooks 使用。

```bash
yarn add statelink
// or
npm install statelink
```

### 使用

结合 React Hooks 完成高复杂度的数据驱动的用户界面。

```ts
import { mixinReact, createStatus } from 'statelink';
import App from './app';
mixinReact(React);

const appState = createState({ ...abc });

export function Demo() {
  return <App appState={appState} />;
}
```
