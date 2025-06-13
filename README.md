# Merklemap Certificate Transparency Search

A cli tool for searching SSL/TLS certificates in the Merklemap certificate transparency database.

## Usage

```bash
./merklemap <query> [options]
```

## Examples

```bash
# Search for certificates for a specific domain
./merklemap example.com

# Search with wildcards
./merklemap "*.github.com"

# Get results in JSON format
./merklemap example.com --json

# Export to CSV
./merklemap example.com --csv

# Paginate through results
./merklemap example.com --page 2
```

## Options

- `-p, --page <num>` - Page number for pagination (default: 0)
- `-j, --json` - Output raw JSON response
- `-q, --quiet` - Suppress colored output
- `--no-header` - Don't display header information
- `--csv` - Output results in CSV format
- `--sort-date` - Sort results by first seen date (newest first)

## Requirements

- `curl` - For API requests
- `jq` - For JSON processing

## Installation

```bash
basher install gnomegl/merklemap
```
