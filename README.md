# jam-docs

Documentation site for [jam-nodes](https://github.com/wespreadjam/jam-nodes), powered by [Mintlify](https://mintlify.com).

## Local Development

```bash
npm i -g mint
mint dev
```

The docs will be available at `http://localhost:3000`.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b docs/my-update`)
3. Edit or add `.mdx` files using [Mintlify MDX format](https://mintlify.com/docs/page)
4. Preview locally with `mint dev`
5. Submit a pull request

## Structure

```
├── index.mdx              # Introduction
├── quickstart.mdx          # Quick start guide
├── creating-nodes.mdx      # Custom node guide
├── mcp.mdx                 # MCP server integration
├── core/                   # Core API reference
├── nodes/                  # Built-in nodes reference
├── editor/                 # Visual editor reference
└── docs.json               # Mintlify configuration
```

## License

MIT
