fork from [IFTTT/dash: A self-contained, mostly zero-configuration environment for developing containerized applications at IFTTT. http://ifttt.github.io](https://github.com/IFTTT/dash)

This script will install the following:

- Homebrew with XCode Command Line Tools
- Homebrew Cask
- Ansible
- Docker
- Docker Machine
- Docker Compose

and will create:

It should run idempotently, meaning you should be able to run it as many times as you want and it won't hurt anything. If it fails due to a temporary condition (like network issues), running it again should pick up where it left off. If new items are added to the script, running it against a functioning environment should only add the new things.

    bash <(curl -fsSL https://raw.githubusercontent.com/miiton/dash/master/bin/bootstrap)

