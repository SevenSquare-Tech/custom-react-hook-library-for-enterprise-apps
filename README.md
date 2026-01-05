# Custom React Hook Library for Enterprise Apps

## Overview

**custom-react-hook-library-for-enterprise-apps** is a comprehensive collection of production-ready React hooks designed to accelerate development in large-scale and enterprise React applications.  
The library provides well-tested, modular hooks covering UI interactions, browser APIs, performance optimizations, state management utilities, and more.

This package is inspired by and based on the open-source project:
https://github.com/antonioru/beautiful-react-hooks

---

## Features

- ⚛️ Designed for React 18+
- 📦 Tree-shakable ESM & CommonJS builds
- 🧠 TypeScript type definitions included
- 🧩 Modular per-hook imports
- 🚀 Enterprise-ready patterns
- 🔁 Supports RxJS & React Router
- 📱 Touch, mouse, drag, swipe & gesture hooks
- 🌐 Browser API integrations (Media, Speech, Geo-location, Storage)

---

## Installation

```bash
npm install custom-react-hook-library-for-enterprise-apps
```

or

```bash
yarn add custom-react-hook-library-for-enterprise-apps
```

---

## Peer Dependencies

You must install the following in your project:

- react >= 18.2.0 < 20
- react-dom >= 18.2.0 < 20
- react-router-dom >= 5
- rxjs >= 7

---

## Usage

Each hook is exported as an individual entry for optimal bundling.

Example:

```ts
import useWindowScroll from "custom-react-hook-library-for-enterprise-apps/useWindowScroll";

const Component = () => {
  const { x, y } = useWindowScroll();
  return <div>Scroll Y: {y}</div>;
};
```

---

## Available Hooks

### Browser & Window

- useWindowScroll
- useWindowResize
- useViewportState
- useViewportSpy
- useMediaQuery
- useOnlineState
- useRenderInfo

### Lifecycle

- useDidMount
- useWillUnmount
- useUnmount
- useLifecycle
- useIsFirstRender
- useUpdateEffect

### State Utilities

- useToggle
- useObjectState
- useMutableState
- useValidatedState
- useDefaultedState
- usePreviousValue
- useValueHistory

### Timers & Performance

- useTimeout
- useInterval
- useRequestAnimationFrame
- useDebouncedCallback
- useThrottledCallback
- useConditionalTimeout

### Storage

- useLocalStorage
- useSessionStorage
- useCookie

### Events

- useEvent
- useGlobalEvent
- useResizeObserver
- useMutationObserver

### Mouse & Touch

- useMouse
- useMouseState
- useMouseEvents
- useTouch
- useTouchState
- useTouchEvents

### Gestures & Drag

- useDrag
- useDragEvents
- useDropZone
- useSwipe
- useSwipeEvents
- useVerticalSwipe
- useHorizontalSwipe
- useLongPress

### Routing & URL

- useQueryParam
- useQueryParams
- useURLSearchParams
- useSearchQuery

### Media & Audio

- useAudio
- useSpeechRecognition
- useSpeechSynthesis
- useSystemVoices

### Sensors & APIs

- useGeolocation
- useGeolocationState
- useGeolocationEvents
- useInfiniteScroll
- useObservable

---

## Build Scripts

```bash
npm run build        # Build CJS, ESM, and types
npm run lint         # Lint source files
npm run test         # Run tests
npm run start        # Start styleguidist server
npm run build-doc    # Build documentation
```

---

## Module Formats

- CommonJS: dist/
- ES Modules: dist/esm/
- TypeScript Types: dist/\*.d.ts
