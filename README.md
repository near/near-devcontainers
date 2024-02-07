# Devcontainer for Near Protocol

This repository hosts the official Devcontainer image for Near Protocol development, featuring preinstalled essential tools. You can access the image on the [GitHub Container Registry](https://ghcr.io/near/near-devcontainer).

## Usage

To incorporate this Devcontainer into your own repositories, follow these steps:

1. Fork the [NEAR Rust Stack template repo](https://github.com/near/cargo-near-new-project-template).
2. Open the forked repository in Codespaces.

For integrating this Devcontainer into your repositories, create the following configuration in `.devcontainer/devcontainer.json`:

```json
{
  "name": "NEAR Devcontainer Rust",
  "image": "ghcr.io/near/near-devcontainer:latest",
  // Uncomment and modify the following lines if necessary
  // "forwardPorts": [8000],
  "customizations": {
    "codespaces": {
      // Uncomment and modify the following lines if necessary
      // "openFiles": ["README.md", "src/lib.rs", "tests/test_basics.rs"]
    }
  }
}
```

## Features

The `near-cli` and `cargo-near` features are available separately and can be used in other Devcontainers. Include the following configurations in your `.devcontainer/devcontainer.json`:

For `cargo-near`:

```json
"features": {
  "ghcr.io/near/near-devcontainers/features/cargo-near:latest": {}
}
```

For `near-cli`:

```json
"features": {
  "ghcr.io/near/near-devcontainers/features/near-cli:latest": {}
}
```

## Contributing

Feel free to contribute to this Devcontainer repository. Any issues or improvements can be raised through the GitHub repository's issue tracker.
