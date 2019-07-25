# wolfram-notebook-embedder

A library to embed [Wolfram Cloud](https://www.wolframcloud.com/) notebooks on other sites. It does *not* use an `<iframe>`, but renders a notebook directly into a given DOM node for a more seamless experience.

## Installation

If you are using a package manager such as [npm](https://www.npmjs.com/get-npm) or [Yarn](https://yarnpkg.com/en/), you can install this package from the npm repository:

    npm install wolfram-notebook-embedder
    
and then import it in your JS code like so:

    import WolframNotebookEmbedder from 'wolfram-notebook-embedder';    
    
You can also import this library as a `<script>` tag from a CDN:

    <script crossorigin src="https://unpkg.com/wolfram-notebook-embedder@0.1/dist/wolfram-notebook-embedder.min.js"></script>
    
and then use the global variable `WolframNotebookEmbedder`.

## Usage & Documentation

* [**Getting Started**](./docs/GettingStarted.md)
* [Library Interface](./docs/LibraryInterface.md)
* [Notebook API](./docs/NotebookAPI.md)
* [Server-Side Rendering](./docs/ServerSideRendering.md)
* [Notebook Loading Phases](./docs/NotebookLoadingPhases.md)
* [Troubleshooting](./docs/Troubleshooting.md)

## Examples

* [Basic Example](./examples/basic.html)
* [Manipulate Example](./examples/manipulate.html)
* [Dimensions Examples](./examples/dimensions.html)
* [Server-Side Rendering](./examples/ssr.html)

## Browser Support

We support all modern browsers (the last two major versions of Chrome, Firefox, Edge, Safari) and Internet Explorer 11. Particularly for IE 11, this library includes an internal "ponyfill" for `Promise`, since this library's API heavily depends on promises.

## Contributing

Everyone is welcome to contribute. Please read the [Contributing guide](CONTRIBUTING.md) and the [Development guide](./docs/Development.md) for more information, including how to run the tests.

## Versioning

We use [semantic versioning](https://semver.org/) for this library and its API.

Each version of this library is compatible with a certain range of versions of the Wolfram Cloud. Currently, the requirement is Wolfram Cloud 1.50 (which has not been released yet) or higher. We try hard not to make any backward-incompatible changes on the Wolfram Cloud side, which would require an update of this library to keep embeddings working.

## License

This project is licensed under the [MIT license](./LICENSE).
