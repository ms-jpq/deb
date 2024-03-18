# PPA

- [Source](https://github.com/ms-jpq/deb-src)

- [Artifacts](https://github.com/ms-jpq/deb)

```bash
curl --disable --fail --location --no-progress-meter -- 'https://raw.githubusercontent.com/ms-jpq/deb/refs/heads/deb/pubkey.asc' | command -- sudo -- gpg --batch --dearmor --yes --output /etc/apt/trusted.gpg.d/ms-jpq.gpg
```

```bash
command -- sudo -- tee -- /etc/apt/sources.list.d/ms-jpq.list <<-'EOF'
deb https://raw.githubusercontent.com/ms-jpq/deb/refs/heads/deb/ /
EOF
```
