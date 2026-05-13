# BasicOps OpenClaw Setup Files

This repository is the public starting point for the BasicOps OpenClaw replication bundle.

If you are new to Linux or headless servers, start here.

## Purpose

This repository lets you create an agent in OpenClaw and connect it to an agent in BasicOps, giving you an AI agent as a team member inside BasicOps.

## Prerequisites

You will need a BasicOps account. If you do not have one, you can sign up for a trial at [app.basicops.com/signup?agents](https://app.basicops.com/signup?agents).

## Before you start

In BasicOps, you need to add an agent and create an API key for it:

1. Select Settings in the left sidebar.
2. Select Users, then click the Agents tab.
3. Click Add Agent, enter the name you want to use, then click Add Agent.
4. A dialog titled Add API Key will appear. Enter a name for the key, for example the agent's name, then click Add API Key.
5. The agent's API key is shown in the next dialog. Copy it and store it somewhere safe, you will need it during setup.

## What is in this repository

The two most important files at the top level are:

- `UNPACK-FIRST.md`
- `basicops-agent-replication-bundle.tar.gz`

## Most common beginner path

Use this path if the target machine already has OpenClaw installed and working.

### Copy this into your server terminal

```bash
git clone https://github.com/BasicOps/openclaw.git
cd openclaw
mkdir -p ~/basicops-agent-bundle
tar -xzf basicops-agent-replication-bundle.tar.gz -C ~/basicops-agent-bundle --strip-components=1
cd ~/basicops-agent-bundle
ls
```

After that, open and follow:

- `~/basicops-agent-bundle/START-HERE.md`
- usually `~/basicops-agent-bundle/INSTALL-WITH-OPENCLAW.md`

## If git is not installed on the server

Use this fallback instead:

```bash
curl -L -o basicops-agent-replication-bundle.tar.gz https://github.com/BasicOps/openclaw/raw/main/basicops-agent-replication-bundle.tar.gz
mkdir -p ~/basicops-agent-bundle
tar -xzf basicops-agent-replication-bundle.tar.gz -C ~/basicops-agent-bundle --strip-components=1
cd ~/basicops-agent-bundle
ls
```

## If you want your local OpenClaw assistant to help from the beginning

That is supported, and usually easier for novices.

After unpacking, the shortest path is usually:

1. open your local OpenClaw assistant
2. tell it to use `~/basicops-agent-bundle/INSTALL-WITH-OPENCLAW.md`
3. expect it to ask only for the agent ID first and choose safe defaults for the rest

## If OpenClaw is not installed yet

Stop there and install OpenClaw first.
After OpenClaw is working, come back to this repository and continue.

## If something goes wrong

Do not guess.
Send the exact command output to the person helping you, or to your local OpenClaw assistant if you already have one running.
