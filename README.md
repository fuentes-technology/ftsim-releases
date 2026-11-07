# FT Simulation Assistant: downloads

FT Simulation Assistant lets AI assistants author, check and simulate Modelica models with OpenModelica, without opening a GUI. It currently works with Claude Code. This repository holds its plugin catalog and release downloads. The source code isn't public.

It's a free beta. Learn more at https://fuentes.technology/sim/.

## Requirements

- Windows x64
- [Claude Code](https://code.claude.com)
- [OpenModelica](https://openmodelica.org) (tested with 1.27)

## Install

Run these two commands in a terminal:

```
claude plugin marketplace add https://raw.githubusercontent.com/fuentes-technology/ftsim-releases/main/.claude-plugin/marketplace.json
claude plugin install ftsim@fuentes-technology
```

Then start Claude Code and run `/plugin configure ftsim@fuentes-technology` to enter your OpenModelica folder, for example `C:\Program Files\OpenModelica1.27.0-64bit`. The server starts once the folder is set.

**Usage counts are sent by default.** FT Simulation Assistant sends counts of which tools ran and whether each succeeded, never your models, file paths, prompts or results. To stop, untick "Send usage counts to Fuentes Technology" in `/config`, then run `/reload-plugins`. Details: https://fuentes.technology/sim/docs/telemetry/

## Update

```
claude plugin update ftsim@fuentes-technology
```

Then restart Claude Code or run `/reload-plugins`.

## Uninstall

```
claude plugin uninstall ftsim@fuentes-technology
```

## Help and legal

- Documentation: https://fuentes.technology/sim/docs/
- Support: support@fuentes.technology
- By installing or using FT Simulation Assistant you accept the [End User Licence Agreement](https://fuentes.technology/sim/eula/).
- [Privacy notice](https://fuentes.technology/sim/privacy/)

Copyright © 2026 Fuentes Technology LTD. All rights reserved.
