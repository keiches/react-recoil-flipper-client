# react-recoil-client

[![NPM](https://img.shields.io/npm/v/react-recoil-client.svg)](https://www.npmjs.com/package/react-recoil-client) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

Flipper React Provider to visualize [Recoil.js](https://recoiljs.org/) atoms and logs of its changes. This package is meant to be used with the `flipper-plugin-react-recoil` plugin from Flipper.

## Install

```bash
yarn add react-recoil-client
```

Or

```bash
npm install --save react-recoil-client
```

## Usage

Simply put the `<FlipperRecoilProvider />` anywhere as a children of the `<RecoilRoot>` to send Recoil.js events to Flipper.

```tsx
import { RecoilRoot } from 'recoil';
import FlipperRecoilProvider from 'react-recoil-client'

const App: React.FC = () => {
  return (
    <RecoilRoot>
      <FlipperRecoilProvider />
      ...
    </RecoilRoot>
  )
}
```

## License

MIT © [BenJeau](https://github.com/BenJeau)
