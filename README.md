# athena-protobufs-dotnet

.NET packaging of the Athena protobufs - provides generated gRPC client and model packages for the Resolver Athena API.

## Packages

| Package | Description |
|---------|-------------|
| `ResolverAthena.Grpc.Client` | Generated gRPC client for the Resolver Athena API |
| `ResolverAthena.Grpc.Models` | Generated gRPC models/messages for the Resolver Athena API |

## Installation

```bash
dotnet add package ResolverAthena.Grpc.Client
```

Or for just the models:

```bash
dotnet add package ResolverAthena.Grpc.Models
```

## Building

This repository uses a git submodule to reference the proto files from [athena-protobufs](https://github.com/crispthinking/athena-protobufs).

```bash
# Clone with submodules
git clone --recursive https://github.com/crispthinking/athena-protobufs-dotnet.git

# Or if already cloned
git submodule update --init --recursive

# Build
dotnet build Resolver.Athena.Grpc.slnx
```

## License

MIT
