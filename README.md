# paint_example
Updated paint example from wasm-bindgen

This is an update to the [paint example](https://github.com/rustwasm/wasm-bindgen/tree/master/examples/paint) from wasm-bindgen.

To build and run do:
```
npm run dev
```

---
# Why?

Just wanted to understand wasm-bindgen, wasm-pack and webpack enough to get rolling with my own rust/wasm paint project that I plan on doing.

I started it in the way I tend to start a new projects which is using a bunch of commands:

```bash
mkdir paint_example &&
cd paint_example &&
npm init &&
npm install --save-dev @wasm-tool/wasm-pack-plugin html-webpack-plugin webpack webpack-cli webpack-dev-server &&
cargo init --lib &&
cargo add js-sys wasm-bindgen web-sys &&
touch index.js &&
touch index.html &&
touch webpack.config.js
```
Then copied the old `lib.rs`, `index.js` and `index.html`
and used my own `webpack.config.js` file. Then edited `Cargo.toml` with by adding the `[lib]` section and copied the `dependencies.web-sys` features from the original project over and added my `script` entry in `package.json`
