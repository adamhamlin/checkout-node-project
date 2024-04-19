# `checkout-node-project`

A simple composite GitHub Action to checkout and initialize a Node project.

## Usage

Remove boilerplate to initialize your node project, so you can replace...

```yaml
steps:
  - name: Checkout your branch
    uses: actions/checkout@v3

  - name: Then install Node.js
    uses: actions/setup-node@v3
    with:
      node-version: 20.x

  - name: Then install dependencies
    run: npm ci
```
with...
```yaml
steps:
  - name: All above steps in one!
    uses: adamhamlin/checkout-node-project@v0.1.0
    with:
      node-version: 20.x
```
