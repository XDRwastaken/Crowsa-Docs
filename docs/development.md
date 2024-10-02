# Create a Project

One thing that makes Crowsa so flexible is it’s ability to work with any HTML builder engine.
There's [to_html](https://github.com/sbsoftware/to_html.cr), Crystal's own [html_builder](https://github.com/crystal-lang/html_builder), [Blueprint](https://github.com/stephannv/blueprint) and many more to choose from to write your HTML code.

To get started, create a Crystal project:

```sh
crystal init app hello_world
```

Then add this line in the application's `shard.yml`:

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

run_app("[config.json"](#run_app))
```

### This section is still a work in progress.
