# Toolboxes

This directory contains a variety of scripts for generating [Toolbox](https://github.com/containers/toolbox) images. Link or copy to required `bin` folders on your `$PATH` (e.g. `$HOME/.local/bin`).

Name | Description
--- | ---
`toolbox-create-base`|Creates the base toolbox image, with basic tools/programs such as the Fish shell and Kakoune
`toolbox-create-go`|Creates a base toolbox image (default-named `go`) and installs Go and Kakoune's LSP client ([kak-lsp](https://github.com/kak-lsp/kak-lsp)) within it.
`toolbox-go-postcreate`| Installs Go tooling currently running to `golangci-lint`, `gopls`, `goimports` and other tools required by Kakoune's basic Go configuration.

The general aim of the toolboxes is to keep all required tooling within the toolbox, so the `$HOME` folder **only** contains data (i.e. code); also, toolbox containers can (and should) be deleted and recreated regularly.
