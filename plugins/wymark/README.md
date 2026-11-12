# Wymark

Wymark is a markdown editor where you review what changed in a document, accept or reject each change, and comment on it. This plugin lets Claude read that review before it edits a file: what changed since your last review, where each change came from, and the comment threads.

This is the macOS plugin. On Windows, add **Wymark for Windows** from the same marketplace instead.

## Install it

In the Claude desktop app (Cowork included): Customize > Plugins > Add > Add marketplace, enter `wymarkapp/wymark`, select Sync, then add Wymark.

In Claude Code:

```
/plugin install wymark --marketplace wymarkapp/wymark
```

## Use it

Wymark must be running, with the `wymark` command turned on and installed from Settings > Review & comments. The plugin starts `wymark mcp` from where Wymark installs it, `/usr/local/bin/wymark`. Then ask Claude to work on a markdown document you review in Wymark; it reads the review first.

## Data

The plugin talks only to Wymark on your computer. What Wymark answers, such as a document's changes and comments, reaches Claude as any tool's answer does; the plugin sends nothing anywhere else.
