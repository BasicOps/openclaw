# Unpack First

This note is meant to live **outside** the archive.
Read it before unpacking `basicops-agent-replication-bundle.tar.gz`.

## What you should have

You should normally receive these two files together:

- `basicops-agent-replication-bundle.tar.gz`
- `UNPACK-FIRST.md`

## Recommended path for most people

If the target machine already has **OpenClaw installed and working**, do this:

### 1. Unpack the bundle

Copy and paste this:

```bash
mkdir -p ~/basicops-agent-bundle
tar -xzf basicops-agent-replication-bundle.tar.gz -C ~/basicops-agent-bundle --strip-components=1
```

### 2. Open the guide inside the bundle

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
