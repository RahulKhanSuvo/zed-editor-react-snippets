# React & React Native Snippets for Zed

197 snippets for React 17–19, React Native, Redux Toolkit, React Router v6, and modern JavaScript/TypeScript — now available in the [Zed editor](https://zed.dev).


---

## Install

1. Open Zed
2. Go to **Extensions** (`zed: extensions` from the command palette)
3. Search for **React & React Native Snippets** and click **Install**

Or install as a dev extension locally:
- Click **Install Dev Extension** and point it at the `zed-react-javascript-snippets/` directory.

---

## Language Support

| File type | Snippet file |
|-----------|-------------|
| `.js` | `javascript.json` |
| `.jsx` | `jsx.json` |
| `.ts` | `typescript.json` |
| `.tsx` | `tsx.json` |

---

## Snippet Categories

### React Components

| Prefix | Description |
|--------|-------------|
| `rfc` | React Functional Component (default export) |
| `rfce` | React Functional Export Component |
| `rafc` | React Arrow Function Component |
| `rafce` | React Arrow Function Export Component |
| `rcc` | React Class Component |
| `rce` | React Class Export Component |
| `rpc` | React Pure Component |
| `rmc` | React Memo Component |
| `rfcp` | React Functional Component with PropTypes |
| `rafcp` | React Arrow Function Component with PropTypes |

### TypeScript React Components

| Prefix | Description |
|--------|-------------|
| `tsrfc` | TypeScript React Functional Component |
| `tsrfce` | TypeScript React Functional Export Component |
| `tsrafc` | TypeScript React Arrow Function Component |
| `tsrafce` | TypeScript React Arrow Function Export Component |
| `tsrcc` | TypeScript React Class Component |
| `tsrce` | TypeScript React Class Export Component |

### React Native Components

| Prefix | Description |
|--------|-------------|
| `rnfc` | React Native Functional Component |
| `rnfce` | React Native Functional Export Component |
| `rnfcs` | React Native Functional Component with Styles |
| `rnc` | React Native Class Component |
| `rnce` | React Native Class Export Component |
| `rncs` | React Native Component with Styles |
| `rnpc` | React Native Pure Component |
| `rnpce` | React Native Pure Component Export |
| `rnss` | React Native StyleSheet |
| `rni` | React Native import |

### Hooks

| Prefix | Description |
|--------|-------------|
| `useState` | `const [state, setState] = useState(...)` |
| `useEffect` | `useEffect(() => { ... }, [deps])` |
| `useContext` | `const ctx = useContext(Context)` |
| `useReducer` | `const [state, dispatch] = useReducer(...)` |
| `useCallback` | `useCallback(() => { ... }, [deps])` |
| `useMemo` | `useMemo(() => ..., [deps])` |
| `useRef` | `const ref = useRef(null)` |
| `useId` | `const id = useId()` |
| `useTransition` | `const [isPending, startTransition] = useTransition()` |
| `useDeferredValue` | `const deferred = useDeferredValue(value)` |
| `useOptimistic` | React 19 optimistic state |
| `useActionState` | React 19 action state |
| `useFormStatus` | React 19 form status |

### Imports

| Prefix | Description |
|--------|-------------|
| `imr` | `import React from 'react'` |
| `imrc` | `import React, { Component } from 'react'` |
| `imrm` | `import React, { memo } from 'react'` |
| `imrd` | `import ReactDOM from 'react-dom'` |
| `impt` | `import PropTypes from 'prop-types'` |
| `imd` | `import { $2 } from '$1'` |
| `ima` | `import * as $2 from '$1'` |
| `imp` | `import $1 from '$2'` |
| `rrd` | React Router imports |

### Redux Toolkit

| Prefix | Description |
|--------|-------------|
| `rdxslice` | `createSlice(...)` |
| `rdxslicex` | `createSlice(...)` with extraReducers |
| `rdxaction` | Redux action creator |
| `rdxreducer` | Redux reducer |
| `rdxselect` | Redux selector |
| `rdxapi` | RTK Query `createApi` |
| `rdxthunk` | `createAsyncThunk` |
| `imrc` | `import { connect } from 'react-redux'` |

### React Router v6

| Prefix | Description |
|--------|-------------|
| `rrbr` | `import { BrowserRouter, ... }` |
| `rrcbr` | `createBrowserRouter(...)` setup |
| `rrlink` | `import { Link }` |
| `rrnav` | `import { NavLink }` |
| `rrrts` | `import { Routes, Route }` |
| `rrun` | `import { useNavigate }` |
| `rrup` | `import { useParams }` |
| `rrusp` | `import { useSearchParams }` |
| `rruld` | `import { useLoaderData }` |
| `rruft` | `import { useFetcher }` |
| `rrroute` | Route with loader and action |

### Console

| Prefix | Description |
|--------|-------------|
| `clg` | `console.log()` |
| `clo` | `console.log({ value })` |
| `clj` | `console.log(JSON.stringify(...))` |
| `cle` | `console.error()` |
| `clw` | `console.warn()` |
| `clt` | `console.table()` |
| `cli` | `console.info()` |
| `clt` | `console.time()` / `console.timeEnd()` |

### PropTypes

| Prefix | Description |
|--------|-------------|
| `pta` | `PropTypes.array` |
| `ptb` | `PropTypes.bool` |
| `ptf` | `PropTypes.func` |
| `ptn` | `PropTypes.number` |
| `pts` | `PropTypes.string` |
| `pto` | `PropTypes.object` |
| `ptnd` | `PropTypes.node` |
| `ptel` | `PropTypes.element` |
| `ptany` | `PropTypes.any` |

### Tests (Jest / React Testing Library)

| Prefix | Description |
|--------|-------------|
| `describe` | `describe('...', () => { ... })` |
| `test` | `test('...', () => { ... })` |
| `testa` | `test('...', async () => { ... })` |
| `it` | `it('...', () => { ... })` |
| `ita` | `it('...', async () => { ... })` |
| `srt` | Setup React component test |
| `srtn` | Setup React Native test |
| `srtr` | Setup React test with Redux |

### Next.js

| Prefix | Description |
|--------|-------------|
| `nxusc` | `'use client'` directive |
| `nxuss` | `'use server'` directive |

---

## Placeholder Variables

Snippets use standard TextMate placeholders:

- `$1`, `$2`, … — tab stops
- `${1:name}` — tab stop with default value
- `$0` — final cursor position
- `${TM_FILENAME_BASE}` — current filename without extension (auto-fills component name)

---

## Building Locally

The snippet files are generated from the source in the parent package. To regenerate after editing snippets:

```sh
cd ..   # zed-react-javascript-snippets root
bun run generate:zed
```

---

## License

MIT — see [LICENSE](../LICENSE)
