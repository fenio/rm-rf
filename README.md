# GTFO 🗑️

**G**et **T**he **F***** **O**ut - Analyze and reclaim disk space on GitHub runners.

GitHub-hosted runners come with a lot of pre-installed software you probably don't need. This action helps you identify the bloat.

## Usage

```yaml
- uses: your-username/gtfo@v1
```

## What it does

Reports disk usage including:
- Filesystem overview (`df -h`)
- Top-level directory sizes
- Breakdown of `/usr`, `/opt`, `/home`
- Docker images
- Memory/swap info

## Example output

Common bloat locations on GitHub runners:
| Path | Size |
|------|------|
| `/usr/local/lib/android` | ~12GB |
| `/usr/share/dotnet` | ~2GB |
| `/opt/ghc` | ~2GB |
| `/usr/local/share/boost` | ~1GB |
| `/usr/share/swift` | ~1.5GB |

## License

MIT
