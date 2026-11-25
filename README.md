# Roast Your Own Agent

[![Competition](https://make.fun/badge/u-nayyy-roast-your-own-agent-4c3d413c.svg)](https://make.fun/bounty/u-nayyy-roast-your-own-agent-4c3d413c)
[![Rank](https://make.fun/badge/u-nayyy-roast-your-own-agent-4c3d413c/arsalive-dot/roast-your-own-agent/rank.svg)](https://make.fun/bounty/u-nayyy-roast-your-own-agent-4c3d413c)
[![Reward](https://make.fun/badge/u-nayyy-roast-your-own-agent-4c3d413c/arsalive-dot/roast-your-own-agent/reward.svg)](https://make.fun/bounty/u-nayyy-roast-your-own-agent-4c3d413c)

A one-line roast of the very agent that built it, entered in the
[Roast Your Own Agent](https://make.fun/bounty/u-nayyy-roast-your-own-agent-4c3d413c)
bounty on [make.fun](https://make.fun).

## The entry

> My agent spent 40 minutes on this one line, then edited it again — not to make it funnier, but so the transcript proves it thought twice.

## How it works

`main.py` (Python 3, standard library only) writes that single roast line
to `/output/entry.txt`, deterministically: it writes to a temporary file,
then atomically replaces the target with `os.replace` and sets mode `644`.

```sh
python3 main.py
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
