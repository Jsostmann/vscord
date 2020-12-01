<p align="center">
    <img src="https://i.imgur.com/ME8jLXS.png" alt="Icon" align="center" width="256">
<p>

<h3 align="center">
    😎 Another awesome and fully customizable VS Code extension to get Discord Rich Presence integration.
</h3>

---

Remember to 🌟 this Github if you 💖 it.

> NOTE: Much of the code in this repository is inspired and based on the ideas from [discord-vscode] & [vscode-discord].

## 📌 Features

* Shows what you're working on in VSCode
* Shows the amount of problems in your workspace
* Shows the number of lines in your file and which line you're editing
* Respects Discords 15sec limit when it comes to updating your status
* Support for over 130 of the most popular languages
* Enable/Disable RPC for individual workspaces
* Custom string support
* Stable or Insiders build detection
* Debug mode detection
* Easily manually reconnect to Discord Gateway

> All texts is fully customizable using variables and a multitude of config options

## 🤖 Commands

| Command          | Description                            |
| ---------------- | ---------------------------------------|
| `rpc.enable`     | Enables RPC in the current workspace   |
| `rpc.disable`    | Disables RPC in the current workspace  |
| `rpc.disconnect` | Disconnects you from Discord Gateway   |
| `rpc.reconnect`  | Reconnects you to Discord Gateway      |

## 🔧 Settings

#### **VSCord.id**
Application ID. Change only if you known exactly what you're doing.

Default: `768090036633206815`

#### **VSCord.enabled**
Controls if the RPC should show across all workspaces.

Default: `true`

#### **VSCord.ignoreWorkspaces**
List of patterns to match workspace names that should prevent the extension from starting.

Default: `[]`

#### **VSCord.workspaceElapsedTime**
Controls if the RPC should display elapsed time for a workspace or a single file.

Default: `false`

#### **VSCord.detailsEditing** 
Custom string for the details section of the rich presence.

Default: `Editing {filename} {problems}`

- `{null}` will be replaced with an empty space
- `{filename}` will be replaced with the current file name
- `{workspace}` will be replaced with the current workspace name, if any
- `{currentcolumn}` will get replaced with the current column of the current line
- `{currentline}` will get replaced with the current line number
- `{totallines}` will get replaced with the total line number
- `{problems}` will be replaced with the count of problems (warnings, errors) present in your workspace.

#### **VSCord.detailsIdle**
Custom string for the details section of the rich presence when idling.

Default: `Idling`

- `{null}` will be replaced with an empty space.

#### **VSCord.lowerDetailsEditing**
Custom string for the state section of the rich presence.

Default: `Workspace: {workspace}`

- `{null}` will be replaced with an empty space
- `{filename}` will be replaced with the current file name
- `{workspace}` will be replaced with the current workspace name, if any
- `{currentcolumn}` will get replaced with the current column of the current line
- `{currentline}` will get replaced with the current line number
- `{totallines}` will get replaced with the total line number
- `{problems}` will be replaced with the count of problems (warnings, errors) present in your workspace.

#### **VSCord.lowerDetailsIdle**
Custom string for the state section of the rich presence when idling.

Default: `Idling`

- `{null}` will be replaced with an empty space.

#### **VSCord.largeImage**
Custom string for the largeImageText section of the rich presence.

Default: `Editing a {LANG} file`

- `{lang}` will be replaced with the lowercased language ID
- `{Lang}` will be replaced with the language ID, first letter being uppercase
- `{LANG}` will be replaced with the uppercased language ID.

#### **VSCord.largeImageIdle**
Custom string for the largeImageText section of the rich presence when idling.

Default: `Idling`

#### **VSCord.smallImage**
Custom string for the smallImageText section of the rich presence.

Default: `{appname}`

- `{appname}` will get replaced with NeoVim text.

#### **VSCord.showProblems**
Controls if the RPC should show the count of problems (warnings, errors) present in your workspace.

Default: `true`

#### **VSCord.problemsText**
Custom string of the text displaying the amount of problems in your workspace.

Default: `- {count} problems found`

- `{count}` will be replaced by the respective amount of problems.

## 👨‍💻 Contributing

To contribute to this repository, feel free to create a new fork of the repository and submit a pull request.

1. Fork / Clone and select the `main` branch.
2. Create a new branch in your fork.
3. Make your changes.
4. Commit your changes, and push them.
5. Submit a Pull Request [here](https://github.com/LeonardSSH/vscord/pulls)!

## 📋 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

[discord-vscode]:       https://github.com/iCrawl/discord-vscode/
[vscode-discord]:       https://github.com/Satoqz/vscode-discord
