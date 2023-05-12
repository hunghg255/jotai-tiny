# jotai-tiny

## Reactjs State Manager with no dependencies

[![npm version](https://badge.fury.io/js/jotai-tiny.svg)](https://badge.fury.io/js/jotai-tiny) [![npm](https://img.shields.io/npm/dw/jotai-tiny.svg?logo=npm)](https://www.npmjs.com/package/jotai-tiny) [![npm](https://img.shields.io/bundlephobia/minzip/jotai-tiny)](https://www.npmjs.com/package/jotai-tiny)
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)

## Demo

[Demo](https://jotai-tiny-demo.vercel.app/)

## Installation

[![NPM](https://nodei.co/npm/jotai-tiny.png?compact=true)](https://nodei.co/npm/jotai-tiny/)

#### Require

```
react >= 18
```

#### To install the latest stable version:

```
npm install --save jotai-tiny
```

#### Basic usage:

```tsx
import { atom, useAtom, useAtomValue } from "jotai-tiny";

const atomCount = atom(0);
const atomCount1 = atom(1);

// const totalCountAtom = atom((get) => get(atomCount) + get(atomCount1));
// const dataAtom = atom(() => fetch("/data.json").then((res) => res.json()));

const App = () => {
  const [count, setCount] = useAtom(atomCount)

  return <>
    <h5>{count}</h5>
    <button onClick={() => setCount(count + 1)}>Click</button>
  </>;
}
```
