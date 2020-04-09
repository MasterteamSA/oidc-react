# OIDC React

[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
[![code style: airbnb](https://img.shields.io/badge/eslint-airbnb-ff5a5f.svg?style=flat-square)](https://github.com/prettier/prettier)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg?style=flat-square)](http://commitizen.github.io/cz-cli/)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg?style=flat-square)](https://github.com/semantic-release/semantic-release)
![Build & Deploy](https://github.com/bjerkio/oidc-react/workflows/Build%20&%20Deploy/badge.svg)

[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/bjerkio/oidc-react.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/bjerkio/oidc-react/context:javascript)
[![codecov](https://codecov.io/gh/bjerkio/oidc-react/branch/master/graph/badge.svg)](https://codecov.io/gh/bjerkio/oidc-react)
[![Maintainability](https://api.codeclimate.com/v1/badges/04b50822a61583ccdb5f/maintainability)](https://codeclimate.com/github/bjerkio/oidc-react/maintainability)
[![Dependabot Status](https://api.dependabot.com/badges/status?host=github&repo=bjerkio/oidc-react&identifier=253005089)](https://dependabot.com)

![oidc-react logo](assets/logo.jpg)

## About

React component (AuthProvider) to provide OpenID Connect and OAuth2 protocol support. Has [hooks](guides/HOOKS.md) 🎉

Based on [oidc-client-js](https://github.com/IdentityModel/oidc-client-js).

## Quickstart

Install packages by running:

```shell
$ npm install oidc-react
```

## Usage

```typescript
...
import { AuthProvider } from 'oidc-react';

const oidcConfig = {
  onSignIn: () => {
    // Redirect?
  },
  authority: 'https://oidc.io/oauth',
  clientId: 'this-is-a-client-id',
  redirectUri: 'https://my-app.com/'
};

const Routes = () => (
  <AuthProvider {...oidcConfig}>
    <Switch>
      <Route exact path="/">
        <Dashboard />
      </Route>
      ...
    </Switch>
  </AuthProvider>
);
```

# Documentation

Apart from this README, you can find details and examples of using the SDK in the following places:

- [SDK Documentation](docs/README.md)
- [Guides](guides/)
- [Example repository](https://github.com/cobraz/example-react-oidc)
- [oidc-client-js Documentation](https://github.com/IdentityModel/oidc-client-js/wiki)

## Contribute & Disclaimer

We love to get help 🙏 Read more about how to get started in [CONTRIBUTING](CONTRIBUTING.md) 🌳
