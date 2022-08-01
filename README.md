# core-typescript

TypeScript will support all proposals above stage-3.  
But there are always some gap between TypeScript support and proposal progress.  
And sometimes we want to use proposals within stage-3 (e.g. `Iterator helper`) because we may use polyfill.  

In this case, we have to write those declarations by our own.
But with `core-typescript`, we can use these proposal with additional declaration files.

## Install

```
pnpm add core-typescript -D
```

## Setup
Set add `core-typescript` into `types` in `compiler options`.

```json
{
  "compilerOptions": {
    "types": ["core-typescript"]
  }
}
```

## Features
- [x] Finished proposals
    - [x] `Array` find from last
- [x] Stage 3 proposals
    - [x] `Array` grouping
    - [x] Change `Array` by copy
- [x] Stage 2 proposals
    - [x] `Iterator` helpers
    - [x] New `Set` methods
    - [x] `Map.prototype.emplace`
    - [x] `Array.fromAsync`
    - [x] `Array.isTemplateObject`
    - [x] `Symbol.{ asyncDispose, dispose }` for `using` statement
    - [x] `Symbol.metadataKey` for decorators metadata proposal
- [ ] Stage 1 proposals
    - [ ] `Observable`
    - [ ] New collections methods
    - [ ] `.of` and `.from` methods on collection constructors
    - [ ] `compositeKey` and `compositeSymbol`
    - [ ] `Array` filtering
    - [ ] `Array` deduplication
    - [ ] Getting last item from `Array`
    - [ ] `Number.range`
    - [ ] `Number.fromString`
    - [ ] `Math` extensions
    - [ ] `Math.signbit`
    - [ ] `String.cooked`
    - [ ] `String.prototype.codePoints`
    - [ ] `Symbol.matcher` for pattern matching
- [ ] Stage 0 proposals
    - [ ] `Function.prototype.unThis`
    - [ ] `Function.{ isCallable, isConstructor }`
    - [ ] `URL`
- [ ] Pre-stage 0 proposals
    - [ ] `Reflect` metadata
