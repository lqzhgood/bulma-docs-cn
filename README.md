##############################################################


感谢 @vmlite  https://v2ex.com/member/vmlite 翻译 v0.9 <br/>
可以访问 https://bulma.zcopy.site 查看




##############################################################

## 这是 Bulma 的中文翻译。可以通过以下链接访问
http://lqzhgood.github.io/bulma-docs-cn

欢迎提交 Issues 改进。


## Building the documentation

The documentation HTML is produced with the Ruby-based `jekyll` tool.

1. Make sure Ruby 2.x is installed.
2. `gem install jekyll`

## Viewing the documentation locally

Then to view the documentation in your local checkout:

1. Before you begin, cd into `docs/` directory, and `cp _config.yml _config.local.yml`. Then edit `_config.local.yml` and change the `url:` value to `http://localhost:4000`. This local config file will be ignored by git.
1. In a separate shell session, `cd` to the `docs/` directory, and do:
```
jekyll serve --incremental --config _config.local.yml
```
This will start an HTTP server at `http://localhost:4000/` that serves the docs built in the `_site` directory; and anytime the docs are rebuilt by you, it will serve the docs site on the fly.
2. In your main shell session where you develop, if you change anything in `docs/` the jekyll server will rebuild those on the fly. But if you change anything about the Bulma SASS or CSS, you need to do `npm run start-docs` to build the docs' CSS before you will see it in the browser. The process running `jekyll serve` will pick up the new CSS automatically.

