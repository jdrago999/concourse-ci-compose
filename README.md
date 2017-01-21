
# Concourse CI with Docker Compose

Run the excellent [Concourse CI](http://concourse.ci) in Docker Compose.

## Setup

### Step 1

Clone this repo.

```bash
git clone -b master <this repo>/concourse-ci-compose.git
```

### Step 2

Run the setup script.

```bash
./setup-workstation
export DOCKERHOST=(this machine's IP address)
docker-compose up -d
```

### Step 3

Update your `/etc/hosts` file.

```bash
echo "127.0.0.1    concourse.local" | sudo tee -a /etc/hosts
```

## Acknowledgement

I found the following gist helpful: https://gist.github.com/colthreepv/6b818cfcf296dc1b5c2cf15eb76a140e
