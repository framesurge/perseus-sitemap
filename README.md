# Perseus Sitemap Plugin

This is a plugin for [Perseus](https://github.com/framesurge/perseus) that generates a sitemap for your app by examining the paths generated at build-time. If you're not using incremental generation, you can stop there and the generated sitemap will automatically have a static alias added for it. However, if you are using incremental generation, this plugin exposes a function that you can add to your server routes to dynamically update that sitemap with the pages that have most recently been incrementally generated.

Although a sitemap is fairly trivial to generate manually by examining `dist/render_conf.json`, incremental generation is quite tricky to work around, so this plugin simplifies both processes. While many sites don't actually need a sitemap, some, especially larger sites, benefit substantially from one. The original use-case of this plugin was to make a sitemap for the Perseus website itself!

*This plugin was developed by the maintainer of Perseus.*

## License

See [[`LICENSE`]].
