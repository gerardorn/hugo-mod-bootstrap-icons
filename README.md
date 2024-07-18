This is a [Hugo module](https://gohugo.io/hugo-modules/) that packages the [Bootstrap icons](https://icons.getbootstrap.com/) ready to be used in Hugo.

You need the Hugo extended version and [Go](https://golang.org/dl/) to use this component.

## Use

Add the component to your Hugo site's config:

```toml
[module]
[[module.imports]]
path = "github.com/gerardorn/hugo-mod-bootstrap-icons"
```

Then call the icon with the `resources.Get` method
```
{{ with resources.Get "icons/bootstrap/bootstrap.svg" }}
  <img src="{{ .RelPermalink }}" alt="Bootstrap" width="32" height="32">
{{ end }}

```

