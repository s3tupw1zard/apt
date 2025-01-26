# apt

This is my own apt repository which I use for my own use.

I add things I cant find as deb file in official repositories or somewhere else.

## Installation of this repo:

### Ubuntu 24.04 Noble Numbat

Create `/etc/apt/keyrings` if not existing:

```bash
sudo mkdir -p /etc/apt/keyrings
```

Download gpg key file into `/etc/apt/keyrings`:

```bash
sudo wget -O /etc/apt/keyrings/s3tupw1zard-apt-noble.gpg https://s3tupw1zard.github.io/apt/dists/noble/Release.gpg
```

Add the noble repository to apt:

```echo "deb [signed-by=/etc/apt/keyrings/s3tupw1zard-apt-noble.gpg] https://s3tupw1zard.github.io/apt/ noble main" | sudo tee /etc/apt/sources.list.d/s3tupw1zard-apt-noble.list```
