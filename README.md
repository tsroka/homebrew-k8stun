# Homebrew Tap for k8stun

This is the official [Homebrew](https://brew.sh/) tap for [k8stun](https://github.com/tsroka/k8stun) - Kubernetes Userspace Network Tunnel.

## Installation

```bash
brew tap tsroka/k8stun
brew install k8stun
```

Or install directly (taps automatically):

```bash
brew install tsroka/k8stun/k8stun
```


## Usage

k8stun requires root privileges to create TUN devices and modify routing:

```bash
# Expose services from the default namespace
sudo k8stun

# Expose services from multiple namespaces
sudo k8stun --namespaces default,production,staging

# See all options
k8stun --help
```

## Updating

```bash
brew update
brew upgrade k8stun
```

## Troubleshooting

If you encounter issues, try:

```bash
brew update
brew reinstall k8stun
```

## License

k8stun is dual-licensed under MIT and Apache 2.0.

