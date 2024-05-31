# Prepare

## icons, pictures

- iconfont: [iconfont](https://www.iconfont.cn/)
- iconpark: [iconpark](https://iconpark.oceanengine.com/official)

## phone size

- [uiiuii](https://uiiiuiii.com/screen/)
 
iPhone 13 Pro size: 844px * 390px

find `ui/global.slint` and change window height| window width

```js
export global ROOT_GLOBAL {
  in-out property <length> window-height : 844px;
  in-out property <length> window-width : 390px;
}
```

## theme color

blue: `#0070cd`, `rgb(0, 112, 205)`

## renovate project

### Cargo.toml
- name
- authors
- description
- dependencies and build-dependencies

```toml
[package]
name = "outlook_example"
version = "0.1.0"
edition = "2021"
authors = ["syf20020816@outlook.com"]
build = "build.rs"
description = "an example for Outlook phone use (SurrealismUI + Slint)"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]
slint = "1.6.0"

[build-dependencies]
slint-build = "1.6.0"
```

### assets

- remove redunct svg|png|... (surrealism.png|surrealism.svg)
- add needed icons
