# Getting Started

## So, What's Crowsa?

Crowsa is a little framework that lets you write Windows applications using [JavaScript](https://simple.wikipedia.org/wiki/JavaScript), [HTML](https://simple.wikipedia.org/wiki/HTML) and [CSS](https://simple.wikipedia.org/wiki/Cascading_Style_Sheets).

## Create a Project

One thing that makes Crowsa so flexible is it’s ability to work with any HTML builder engine.
There's [to_html](https://github.com/sbsoftware/to_html.cr), [html_builder](https://github.com/crystal-lang/html_builder), [Blueprint](https://github.com/stephannv/blueprint) and alot more to choose from to write your HTML code from Crystal.

To get starting, first make a Crystal project:

```sh
crystal init app hello_world
```

To use Crowsa in that project, add this line to the application's `shard.yml`:

```yaml
dependencies:
  crowsa:
    git: https://codeberg.org/XDR/Crowsa
```

Then in `src/main.rs`, add these lines:

```crystal
require "crowsa/cli"
require "crowsa/gui/macro"
require "crowsa/gui/run"
require "crowsa/main"
```

## Prerequisites

Funny thing, all Crowsa needs is just the system's webview.

* On Linux, [webkitgtk](https://repology.org/project/webkitgtk/versions) may not be installed, you can install it easily via your package manager.

* While on Windows, you need Microsoft Edge's [WebView2](https://developer.microsoft.com/en-us/microsoft-edge/webview2/?form=MA13LH#download) installed.

For [MacOS](https://i.ytimg.com/vi/hJvW2bg_PFY/maxresdefault.jpg)...