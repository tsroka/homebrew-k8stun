# Homebrew Tap for kpipe

This is the official [Homebrew](https://brew.sh/) tap for [k8stun](https://github.com/tsroka/kpipe) - Kubernetes Userspace Network Tunnel.

## Installation

```bash
brew tap tsroka/kpipe
brew install kpipe
```

Or install directly (taps automatically):

```bash
brew install tsroka/kpipe/kpipe
```


## Usage

k8stun requires root privileges to create TUN devices and modify routing:

```bash
# Expose services from the default namespace
sudo kpipe

# Expose services from multiple namespaces
sudo kpipe --namespaces default,production,staging

# See all options
kpipe --help
```

## Updating

```bash
brew update
brew upgrade kpipe
```

## Troubleshooting

If you encounter issues, try:

```bash
brew update
brew reinstall kpipe
```

## License

k8stun is dual-licensed under MIT and Apache 2.0.

