# Test repository

This repository is a test project to reproduce the error trying to solve at
the following URL.

https://github.com/timocov/dts-bundle-generator/pull/115

## How to reproduce

npm install
npm run build

The following errors are displayed

    Compiling input files...
    Processing ./dist/src/input.d.ts
    Writing ./dist/src/input.d.ts -> dist/output.d.ts
    Checking generated files...
    dist/output.d.ts(3,1): error TS1046: Top-level declarations in .d.ts files must start with either a 'declare' or 'export' modifier.
    
    Error: Compiled with errors
    npm ERR! code ELIFECYCLE
    npm ERR! errno 1
    npm ERR! @ build: `npm run clean && tsc && dts-bundle-generator -o dist/output.d.ts ./dist/src/input.d.ts`
    npm ERR! Exit status 1
    npm ERR!
    npm ERR! Failed at the @ build script.
    npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in: