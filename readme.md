# Webview for nim

Nim bindings for [zserge's Webview](https://github.com/zserge/webview) which is an
excellent cross-platform single header webview
library for C/C++ using Gtk, Cocoa or MSHTML
repectively.

# Docs

Documentation is [here](http://htmlpreview.github.io/?https://github.com/oskca/webview/blob/master/docs/webview.html)

and [Golang's doc for webview](https://godoc.org/github.com/zserge/webview) is
also very useful.

On `debian/ubuntu`, install the webkit2gtk dev package:
- Ubuntu 24.04+: `libwebkit2gtk-4.1-dev`
- Older versions: `libwebkit2gtk-4.0-dev`

The build auto-detects which version is available (preferring 4.1).
To force a specific version, compile with: `nim c -d:webkitPkg=webkit2gtk-4.0 yourapp.nim`
