# hugo-mastodon-embed

Shortcode to embed Mastodon toots

# Installation

## Hugo Module

1. Add the repository as a Hugo module

```
hugo mod get github.com/ericswpark/hugo-mastodon-embed
```

2. Add to your `config.toml`:

```toml
# Modules
[module]
  # Other module imports here...
  [[module.imports]]
    path = "github.com/ericswpark/hugo-mastodon-embed"
    disable = false
```

## Git Submodule (deprecated)

1. Add the repository as a submodule

```
git submodule add https://github.com/ericswpark/hugo-mastodon-embed.git themes/hugo-mastodon-embed
```

2. Add `hugo-mastodon-embed` as a theme in your `config.toml`:

```
theme = ["hugo-mastodon-embed", "default-theme-name"]
```

# Usage

Add the following snippet where you want to embed a Mastodon toot:

```
{{< mastodon server_base="tilde.zone" username="ericswpark" toot_id="109522335209661741" >}}
```

If the default width of 800 is too big, you can change it:

```
{{< mastodon server_base="tilde.zone" username="ericswpark" toot_id="109522335209661741" width="400" >}}
```