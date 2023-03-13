<div align="center">
    <h1>GitSync</h1>
    <p>Sync your Minecraft server's scripts with a Github repository.</p>
    <a href="https://github.com/Baezor1/gitsync/issues"><img src="https://img.shields.io/github/issues/Baezor1/gitsync"></a>
    <a href="https://github.com/Baezor1/gitsync/"><img src="https://img.shields.io/github/forks/Baezor1/gitsync"></a>
    <a href="https://github.com/Baezor1/gitsync/"><img src="https://img.shields.io/github/stars/Baezor1/gitsync"></a>
</div>

## What is GitSync?
GitSync is a simple script that allows you to use Github in Skript workflow.

## Frequently Asked Questions
- Will this work with a private repository? **Yes!**
- Can you connect multiple repositories? **Yes!**
- Can you change the messages and language? **Yes! There is a lang.yml file!**

## Installation
1. Install Plugin Dependencies
    - skript-reflect
    - skript-yaml
    - Skent
2. Install JGit
    - Download the library in the `/libs/` folder in this repository.
    - Drag the library into the `/plugins/skript-reflect/` folder on your Minecraft server.
    - Restart your server.
3. Install `gitsync.sk` in your server's `/plugins/Skript/scripts/` folder.
4. Run `/sk reload gitsync` on your server to generate configurations.

## Configuration

### Authentication
In order to use GitSync, you must connect your Github account. You must input your username and a Github access token!

`config.yml`
```yml
auth:
    username: insert_username
    token: insert_token
```

### Adding Repositories

`config.yml`
```yml
repositories:
    example-name:
        url: Baezor1/Example
        branch: main
        target: synced/
```