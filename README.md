### 概要
- Yjs + Nextのサンプルを動くところまで修正.
- Nextの最新でやったサンプルがなかったので追加.
- y-websocket のimportでエラーになるので、`tsconfig.ts` を修正した

```diff
+ "resolvePackageJsonExports": false,
```

### このプロジェクトをどうやってつくったか
```bash
$ npx create-next-app@latest --ts
$ yarn add y-prosemirror yjs y-websocket @tiptap/core @tiptap/starter-kit @tiptap/react @tiptap/extension-collaboration @tiptap/extension-collaboration-cursor @tiptap/pm
```

### 起動方法
```
$ npx y-websocket start
$ yarn dev
```
### 備考
- サーバー側も追加したい
