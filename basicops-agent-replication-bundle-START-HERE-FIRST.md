# BasicOps Agent Bundle, Start Here First

This note is meant to live **outside** the archive.
It exists so you can see the first step **before** unpacking `basicops-agent-replication-bundle.tar.gz`.

## What you should have

You will usually use one of these two paths:

1. clone this public repository on the target machine
2. or manually copy these two files to the target machine:
   - `basicops-agent-replication-bundle.tar.gz`
   - `basicops-agent-replication-bundle-START-HERE-FIRST.md`

## Recommended path for most people

If the target machine already has **OpenClaw installed and working**, do this:

### 1. Get the files onto the target machine

If `git` is available, use this:

```bash
git clone https://github.com/BasicOps/openclaw.git
cd openclaw
```

If you already copied the files manually, skip that and continue.

### 2. Unpack the bundle

Copy and paste this:

```bash
mkdir -p ~/basicops-agent-bundle
tar -xzf basicops-agent-replication-bundle.tar.gz -C ~/basicops-agent-bundle --strip-components=1
```

### 3. Open the guide inside the bundle

Then read:

- `~/basicops-agent-bundle/START-HERE.md`

For most users, the next file to follow is:

- `~/basicops-agent-bundle/INSTALL-WITH-OPENCLAW.md`

That path is intentionally the shortest and most novice-friendly one.

## If OpenClaw is not installed yet

Stop there and install OpenClaw first.
After OpenClaw is working, come back to this bundle and follow the steps above.

## If something goes wrong while unpacking

Do not guess.
Send the exact command output to the person who sent you this bundle, or to your local OpenClaw assistant if you already have one running.

## Why this file exists

Earlier users got stuck because the unpack instructions were only available **inside** the archive.
That is annoying, and this file fixes it.
