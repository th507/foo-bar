# foo-bar
A test module that demonstrates the quirk of npm@3

## Install
```bash
$ npm install @th507/foobar
```

## Problem
With npm@3, run `npm ls` after installation yields errors
```
@th507/foobar@0.0.0 /Users/john/foo-bar
├─┬ @th507/bar@0.0.0
│ └── UNMET DEPENDENCY @th507/foo@^2.0.0
└── @th507/foo@1.0.0
```

With npm@2, it works as expected
```
@th507/foobar@0.0.0 /Users/john/foo-bar
├─┬ @th507/bar@0.0.0
│ └── @th507/foo@2.0.0
└── @th507/foo@1.0.0
```
