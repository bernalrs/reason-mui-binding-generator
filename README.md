# Reason Mui Binding Generator

This library generates bindings for
[material-ui](https://material-ui-1dab0.firebaseapp.com/). It's automatically generated by an adaption of  [reason-rt-binding-generator](https://github.com/astrada/reason-rt-binding-generator) (created by [astrada](https://github.com/astrada)).

## Prerequisites

Clone & rename the `env.example.js` in the `scripts` folder and enter the path to your `material-ui` **master clone** (this is **not** the NPM version!!).

1. If you don't have the OCaml compiler (or OPAM) installed, please [install
   it](http://opam.ocaml.org/doc/Install.html).

       opam install jbuilder yojson

2. Install
   [reason-cli](https://reasonml.github.io/guide/editor-tools/global-installation#recommended-through-npmyarn).

3. Install JS dependencies:

       yarn install

## How to (re)generate bindings
    yarn extract
    ./rebuild.sh
    
## Todo

- [x] ~~Expose a nested `Colors` module~~ (2017-11-15)
- [ ] Think of a way to use `theme => object` pattern as `withStyles` argument
- [ ] Add `WithTheme` component
- [ ] Add `ThemeProvider` component
- [x] ~~Implement classname overrides~~ (2017-11-15)
- [ ] Apply default values to generation script
- [ ] Implement ref function signatures
- [ ] Ignore "theme" prop in generation
- [ ] Implement array resolving (esp. for union arrays)