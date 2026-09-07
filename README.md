# React-Awesome ⚛️

> A curated list of useful tools, libraries, UI kits, and resources for **React** (web) + **React Native** (mobile).

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

React and React Native share a component model but have very different ecosystems. This repo collects the best-in-class libraries for both — from full design systems like [EUI](https://github.com/elastic/eui) to navigation, state, forms, animation, testing, and Expo tooling.

## Contents

- [React — UI / Design Systems](#react--ui--design-systems)
- [React — Styling](#react--styling)
- [React — Headless / Primitives](#react--headless--primitives)
- [React — Data Tables / Data Grid](#react--data-tables--data-grid)
- [React — Charts / Visualization](#react--charts--visualization)
- [React — Forms](#react--forms)
- [React — State Management](#react--state-management)
- [React — Data Fetching / Server State](#react--data-fetching--server-state)
- [React — Routing](#react--routing)
- [React — Animation / Motion](#react--animation--motion)
- [React — Testing / DevTools](#react--testing--devtools)
- [React Native — UI Kits](#react-native--ui-kits)
- [Cross-Platform (Web + Native)](#cross-platform-web--native)
- [React Native — Navigation](#react-native--navigation)
- [React Native — Core Utilities](#react-native--core-utilities)
- [Expo Ecosystem](#expo-ecosystem)
- [Build / Tooling](#build--tooling)
- [Contributing](#contributing)

---

## React — UI / Design Systems

> Full component libraries with theming, a11y, and docs.

- [Elastic EUI](https://github.com/elastic/eui) — Elastic UI Framework. Production-grade React components, theming, and styling utilities used by Kibana/Elastic.
- [MUI (Material UI)](https://github.com/mui/material-ui) — Most popular React Material implementation. Components, theming, Data Grid, date pickers.
- [Ant Design](https://github.com/ant-design/ant-design) — Enterprise-class UI language + components.
- [Chakra UI](https://github.com/chakra-ui/chakra-ui) — Accessible, composable components with style props.
- [Mantine](https://github.com/mantinedev/mantine) — Full-featured library with hooks, forms, and 100+ components.
- [NextUI / HeroUI](https://github.com/heroui-inc/heroui) — Tailwind-based beautiful components.
- [Blueprint](https://github.com/palantir/blueprint) — Palantir's desktop-oriented UI toolkit.
- [Carbon](https://github.com/carbon-design-system/carbon) — IBM's design system for React.
- [Primer React](https://github.com/primer/react) — GitHub's design system components.
- [shadcn/ui](https://github.com/shadcn-ui/ui) — Copy-paste Radix + Tailwind components. Not a package, a pattern.

## React — Styling

- [Tailwind CSS](https://github.com/tailwindlabs/tailwindcss) — Utility-first CSS framework, de-facto standard with React.
- [styled-components](https://github.com/styled-components/styled-components) — CSS-in-JS with tagged template literals.
- [Emotion](https://github.com/emotion-js/emotion) — Performant CSS-in-JS, used by MUI.
- [Stitches](https://github.com/stitchesjs/stitches) — Near-zero-runtime CSS-in-JS.
- [Vanilla Extract](https://github.com/vanilla-extract-css/vanilla-extract) — Zero-runtime, TypeScript-first CSS.
- [Panda CSS](https://github.com/chakra-ui/panda) — Build-time CSS-in-JS from Chakra team.

## React — Headless / Primitives

> Unstyled, accessible behavior — bring your own styles.

- [Radix Primitives](https://github.com/radix-ui/primitives) — Low-level accessible primitives. Basis for shadcn/ui.
- [Headless UI](https://github.com/tailwindlabs/headlessui) — Tailwind team's unstyled components.
- [React Aria / Adobe Spectrum](https://github.com/adobe/react-spectrum) — Accessibility-first hooks + components.
- [Ark UI](https://github.com/chakra-ui/ark) — Headless components for multiple frameworks including React.
- [Downshift](https://github.com/downshift-js/downshift) — Primitives for autocomplete/combobox/select.

## React — Data Tables / Data Grid

- [TanStack Table](https://github.com/TanStack/table) — Headless table logic, framework-agnostic, hugely popular.
- [MUI X Data Grid](https://github.com/mui/mui-x) — Feature-rich commercial-grade grid.
- [AG Grid React](https://github.com/ag-grid/ag-grid) — Enterprise data grid with React wrapper.
- [React Data Grid](https://github.com/adazzle/react-data-grid) — Lightweight Excel-like grid.

## React — Charts / Visualization

- [Elastic Charts](https://github.com/elastic/elastic-charts) — Companion to EUI for Elastic-style visualizations.
- [Recharts](https://github.com/recharts/recharts) — Composable charting on top of D3.
- [Victory](https://github.com/FormidableLabs/victory) — Formidable's charting suite.
- [Nivo](https://github.com/plouc/nivo) — Rich dataviz on D3 + React.
- [Visx](https://github.com/airbnb/visx) — Airbnb's low-level visualization primitives.
- [React Flow / XYFlow](https://github.com/xyflow/xyflow) — Node-based graphs, diagrams, workflows.

## React — Forms

- [React Hook Form](https://github.com/react-hook-form/react-hook-form) — Performant, uncontrolled forms with minimal re-renders.
- [Formik](https://github.com/jaredpalmer/formik) — Classic declarative form library.
- [TanStack Form](https://github.com/TanStack/form) — Type-safe, framework-agnostic form state.
- [Zod](https://github.com/colinhacks/zod) — Schema validation, pairs perfectly with hook-form.
- [Yup](https://github.com/jquense/yup) — Schema validation predecessor, still widely used.

## React — State Management

- [Zustand](https://github.com/pmndrs/zustand) — Minimal, hook-based store. Recommended default.
- [Jotai](https://github.com/pmndrs/jotai) — Atomic state from Poimandres team.
- [Redux Toolkit](https://github.com/reduxjs/redux-toolkit) — Official batteries-included Redux.
- [Recoil](https://github.com/facebookexperimental/Recoil) — Meta's experimental atom model (in maintenance).
- [Valtio](https://github.com/pmndrs/valtio) — Proxy-based mutable state.
- [XState](https://github.com/statelyai/xstate) — State machines + statecharts for complex flows.

## React — Data Fetching / Server State

- [TanStack Query](https://github.com/TanStack/query) — Server-state standard: caching, retries, invalidation.
- [SWR](https://github.com/vercel/swr) — Vercel's stale-while-revalidate hook.
- [RTK Query](https://github.com/reduxjs/redux-toolkit) — Data fetching built into Redux Toolkit.
- [Apollo Client](https://github.com/apollographql/apollo-client) — GraphQL client standard.
- [urql](https://github.com/urql-graphql/urql) — Lightweight GraphQL client.
- [tRPC](https://github.com/trpc/trpc) — End-to-end typesafe APIs without schemas.

## React — Routing

- [React Router](https://github.com/remix-run/react-router) — De-facto standard router for React SPAs.
- [TanStack Router](https://github.com/TanStack/router) — Type-safe, modern router with caching.
- [Next.js App Router](https://github.com/vercel/next.js) — File-based routing + RSC framework.
- [Wouter](https://github.com/molefrog/wouter) — Tiny 2KB router alternative.

## React — Animation / Motion

- [Framer Motion / Motion](https://github.com/framer/motion) — Declarative layout + gesture animations.
- [React Spring](https://github.com/pmndrs/react-spring) — Spring-physics animations.
- [Auto-Animate](https://github.com/formkit/auto-animate) — Zero-config transitions.
- [Lottie React](https://github.com/LottieFiles/lottie-react) — Render After Effects animations.

## React — Testing / DevTools

- [Testing Library (React)](https://github.com/testing-library/react-testing-library) — User-centric component testing.
- [Vitest](https://github.com/vitest-dev/vitest) — Fast Vite-native test runner.
- [Playwright](https://github.com/microsoft/playwright) — E2E testing standard.
- [Storybook](https://github.com/storybookjs/storybook) — Isolated component workshop/docs.
- [React DevTools](https://github.com/facebook/react/tree/main/packages/react-devtools) — Official profiler/inspector extension.

---

## React Native — UI Kits

- [React Native Paper](https://github.com/callstack/react-native-paper) — Material Design for RN.
- [React Native Elements](https://github.com/react-native-elements/react-native-elements) — Cross-platform toolkit (maintenance mode, still widely used).
- [NativeBase](https://github.com/GeekyAnts/NativeBase) — Accessible component library (v3 maintenance).
- [UI Kitten](https://github.com/akveo/react-native-ui-kitten) — Eva Design-based components.
- [Tamagui UI](https://github.com/tamagui/tamagui) — High-perf universal UI (see Cross-Platform).
- [React Native Reusables](https://github.com/mrzachnugent/react-native-reusables) — shadcn-style universal components.

## Cross-Platform (Web + Native)

> Share code between React DOM and React Native.

- [Tamagui](https://github.com/tamagui/tamagui) — UI + optimizing compiler for RN + Web.
- [NativeWind](https://github.com/marklawlor/nativewind) — Tailwind CSS for React Native.
- [Unistyles](https://github.com/jpudysz/react-native-unistyles) — Fast C++ styling engine.
- [Dripsy](https://github.com/nandorojo/dripsy) — Theme-UI for cross-platform.
- [Solito](https://github.com/nandorojo/solito) — Unified navigation for Next.js + Expo.
- [Expo Router + Next.js](https://github.com/expo/expo) — File-based universal routing story.

## React Native — Navigation

- [React Navigation](https://github.com/react-navigation/react-navigation) — Standard stack/tab/drawer navigation.
- [Expo Router](https://github.com/expo/expo/tree/main/packages/expo-router) — File-based routing on top of React Navigation.
- [React Native Screens](https://github.com/software-mansion/react-native-screens) — Native navigation primitives.
- [React Native Navigation (Wix)](https://github.com/wix/react-native-navigation) — True-native alternative.

## React Native — Core Utilities

- [Async Storage](https://github.com/react-native-async-storage/async-storage) — Persistent key-value storage.
- [MMKV](https://github.com/mrousavy/react-native-mmkv) — Ultra-fast key-value storage.
- [React Native Reanimated](https://github.com/software-mansion/react-native-reanimated) — 60fps UI-thread animations.
- [Gesture Handler](https://github.com/software-mansion/react-native-gesture-handler) — Native gestures.
- [Skia](https://github.com/Shopify/react-native-skia) — Shopify's high-perf 2D graphics.
- [Vision Camera](https://github.com/mrousavy/react-native-vision-camera) — Powerful camera library.
- [Maps](https://github.com/react-native-maps/react-native-maps) — Native map components.
- [WebView](https://github.com/react-native-webview/react-native-webview) — In-app browser views.
- [SVG](https://github.com/software-mansion/react-native-svg) — SVG rendering support.
- [FlashList](https://github.com/Shopify/flash-list) — Shopify's fast list replacement for FlatList.
- [Victory Native](https://github.com/FormidableLabs/victory-native) — Charts for React Native (Skia-based XL).
- [Gifted Charts](https://github.com/Abhinandan-Kushwaha/react-native-gifted-charts) — Simple RN charting.

## Expo Ecosystem

- [Expo SDK](https://github.com/expo/expo) — Managed toolchain, OTA updates, modules, EAS.
- [Expo Router](https://github.com/expo/expo/tree/main/packages/expo-router) — File routing for native apps.
- [Expo Image](https://github.com/expo/expo/tree/main/packages/expo-image) — Performant image component.
- [EAS Build / Update](https://github.com/expo/eas-cli) — Cloud builds + OTA updates.

## Build / Tooling

- [Vite](https://github.com/vitejs/vite) — Fast dev server/bundler for React web.
- [Next.js](https://github.com/vercel/next.js) — Full-stack React framework.
- [Remix / React Router v7](https://github.com/remix-run/react-router) — Full-stack routing framework.
- [Expo](https://github.com/expo/expo) — Toolchain for React Native.
- [Metro](https://github.com/facebook/metro) — RN bundler.
- [Tamagui Compiler](https://github.com/tamagui/tamagui) — Optimizing compiler for universal UI.
- [ESLint React Plugins](https://github.com/jsx-eslint/eslint-plugin-react) — Linting for React.
- [Prettier](https://github.com/prettier/prettier) — Opinionated formatter.

---

## Contributing

PRs welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before adding a library.

Rules of thumb:

1. No tutorials/courses — only tools, libs, frameworks.
2. Must be maintained or widely used (check stars, last commit).
3. One-line description + link. Keep it factual.
4. Put React Native-specific libs under RN sections, universal libs under Cross-Platform.

## License

[MIT](LICENSE) © Amr Elghadban
