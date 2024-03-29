# Changelog

This file was generated using [@jscutlery/semver](https://github.com/jscutlery/semver).

# [5.1.0](https://github.com/k9n-dev/scully-plugins/compare/scully-plugin-mermaid-5.0.0...scully-plugin-mermaid-5.1.0) (2023-11-13)


### Features

* allow versions greater than 13.0.0 for scully plugins ([d9d30e2](https://github.com/k9n-dev/scully-plugins/commit/d9d30e211869874cb59984f61123b2eb900cdf50))



# [5.0.0](https://github.com/k9n-dev/scully-plugins/compare/scully-plugin-mermaid-4.0.1...scully-plugin-mermaid-5.0.0) (2021-12-19)


### Features

* migrate to k9n org ([e42169f](https://github.com/k9n-dev/scully-plugins/commit/e42169fcf875c76725775fa22155451105efbbd2))


### BREAKING CHANGES

* moved packages into `@k9n` org.
notes: please adjust your imports to `@k9n/scully-plugin-*`



## [4.0.1](https://github.com/k9n-dev/scully-plugins/compare/scully-plugin-mermaid-4.0.0...scully-plugin-mermaid-4.0.1) (2021-12-19)



# [4.0.0](/compare/scully-plugin-mermaid-3.0.0...scully-plugin-mermaid-4.0.0) (2021-12-12)



# [3.0.0](/compare/scully-plugin-mermaid-2.0.0...scully-plugin-mermaid-3.0.0) (2021-12-12)



# [2.0.0](/compare/scully-plugin-mermaid-1.0.0...scully-plugin-mermaid-2.0.0) (2021-12-12)



# 1.0.0 (2021-12-12)


### Features

* build plugins with tsc on prepublishOnly bb1d475



## [3.0.0](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v2.0.1...v3.0.0) (2021-05-14)


### ⚠ BREAKING CHANGES

* drop support for angular 10 and earlier

* drop angular 10 support for next version ([ef648b5](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/ef648b5f63d4f927d858fbc3d20adbc98c28c6e5))

### [2.0.1](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v2.0.0...v2.0.1) (2021-05-14)

## [2.0.0](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v1.0.0...v2.0.0) (2020-11-12)


### ⚠ BREAKING CHANGES

* Drop support for Angular 9

### Features

* update to peerDependencies to support Angular 11 ([da6d559](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/da6d55917ac994f57877b942debc34810071aec8))

## [1.0.0](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.9...v1.0.0) (2020-09-21)


### ⚠ BREAKING CHANGES

* The configuration no longer only passes through the `MermaidAPI.Config`. This is now wrapped into the `config` key in the new interface `MermaidPluginConfig` that holds more options.

**Old**:
```
import MermaidAPI from 'mermaid/mermaidAPI';

// ...

const mermaidOptions: MermaidAPI.Config = {
  theme: 'dark',
};
```

**New**:
```
import { /* ... */, MermaidPluginConfig } from '@k9n/scully-plugin-mermaid';

// ...

const mermaidOptions: MermaidPluginConfig = {
  // ... other config options
  config: { theme: 'dark' }
};
```

### Features

* allow to define the selector for mermaid content ([fd8c59d](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/fd8c59d09edac1da04f52d20181a526aac393ab0)), closes [#2](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/issues/2)
* allow to define the wrapper-element ([3209e0c](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/3209e0ca39e1e7e9c1bd33aeadc8d65ed54bffcb)), closes [#3](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/issues/3)


### Bug Fixes

* export MermaidPluginConfig ([fed8729](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/fed8729e2dddc8abfb89af0fea35b623f0935e9d))
* make config params optional ([6f94fe4](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/6f94fe4dffd788a5e053adb2bdaf048e8387a15f))
* replace the whole `pre`-Element ([5f7915a](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/5f7915aa10c168fd1e1bc0a35366e6cebe06c794)), closes [#1](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/issues/1)

### [0.0.10](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.9...v0.0.10) (2020-09-20)


### Features

* allow to define the selector for mermaid content ([29e4afa](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/29e4afade0d3c922e529db0cd9d799ce204f2ea1)), closes [#2](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/issues/2)
* allow to define the wrapper-element ([a03679f](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/a03679f452e97852b7da98a7eaff0bb8694ea2c9)), closes [#3](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/issues/3)


### Bug Fixes

* make config params optional ([bdbea04](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/bdbea04a87ffd64deff4604048b6ad4b15d200b9))
* replace the whole `pre`-Element ([5f7915a](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/5f7915aa10c168fd1e1bc0a35366e6cebe06c794)), closes [#1](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/issues/1)

### [0.0.9](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.8...v0.0.9) (2020-09-13)

### [0.0.8](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.7...v0.0.8) (2020-09-12)


### Bug Fixes

* replace whole `pre` element ([469acba](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/469acba181b481ac7319f5c601c13e7ccacdaf6b))

### [0.0.7](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.6...v0.0.7) (2020-09-12)

### [0.0.6](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.5...v0.0.6) (2020-09-12)

### [0.0.5](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.4...v0.0.5) (2020-09-12)

### [0.0.4](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.3...v0.0.4) (2020-09-12)

### [0.0.3](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/compare/v0.0.2...v0.0.3) (2020-09-12)


### Bug Fixes

* do not insert svg inside `pre`-element ([f59dff7](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/f59dff73ee017856f598fe621061e548263a5e5f))

### 0.0.2 (2020-09-11)


### Features

* initial version ([785c10e](https://github.com/k9n-dev/scully-plugins/tree/main/scully/plugins/scully-plugin-mermaid/commit/785c10e5b4ed4eb0f22b7106218aa27c64dcdac7))
