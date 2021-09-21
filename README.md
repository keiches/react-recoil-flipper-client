# react-recoil-flipper-client

[![NPM](https://img.shields.io/npm/v/react-recoil-flipper-client.svg)](https://www.npmjs.com/package/react-recoil-flipper-client) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

Flipper React Provider to visualize [Recoil.js](https://recoiljs.org/) atoms and logs of its changes. This package is meant to be used with the `[flipper-plugin-react-recoil](https://github.com/BenJeau/flipper-plugin-react-recoil)` plugin, it must be installed from within Flipper.

## Install

```bash
yarn add react-recoil-flipper-client
```

Or

```bash
npm install --save react-recoil-flipper-client
```

## Usage

Simply put the `<RecoilFlipperClient />` anywhere as a children of the `<RecoilRoot>` to send Recoil.js events to Flipper.

```tsx
import { RecoilRoot } from 'recoil';
import RecoilFlipperClient from 'react-recoil-flipper-client'

const App: React.FC = () => {
  return (
    <RecoilRoot>
      <RecoilFlipperClient />
      ...
    </RecoilRoot>
  )
}
```

## License

MIT © [BenJeau](https://github.com/BenJeau)
