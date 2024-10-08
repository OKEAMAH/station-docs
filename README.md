# Station Docs

<div align="center">
  <a href="https://docs.station.money/">
    <img src="static/img/twitter-card-docs.png" width=500>
  </a>
</div>

---


Welcome to the official Station documentation. 


To contribute to this documentation, please read the [Code of Conduct](./DOCS_CODE_OF_CONDUCT.md) and the [Docs Style Guide](./DOCS_STYLE_GUIDE.mdx) before opening a pull request. 


## Setup

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.

## Syntax

### Admonitions

You can use admonitions by importing them and using the following syntax:

```
import Admonition from '@theme/Admonition';

<Admonition type="note" icon="📝" title="Your Title">

Some **content** with _markdown_ `syntax`.

</Admonition>
```

The `icon` and `title` values are optional.

Admonition types:

```
note
tip
info
caution
danger
```

### Details

For dropdown details, use the following syntax:

<details> 
<summary> example </summary>
<p>

```
hidden content
```

</p>
</details>

````
<details>
<summary> Title </summary>
<p>

```
hidden content
```
</p>
</details>
````

### Comments

```
{/*
this is a comment in mdx
*/}
```

## License

This repository is licensed under the Apache license. See [LICENSE](./LICENSE) for full disclosure.

© 2023 Terraform Labs, PTE