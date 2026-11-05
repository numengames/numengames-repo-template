# numengames-repo-template

Starting point for every new Numen Games repository: entry file, owner and shared CI hooks.

It carries **no licence on purpose**: the licence depends on what the repository holds
(PRI-005, STD-010 in [numinia-archive](https://github.com/numengames/numinia-archive)),
and it has to be there from the first commit, because a public repository makes its
promise the moment it is pushed.

## Which licence

| The repository holds | Licence | Also |
|---|---|---|
| A program that runs a service, or the core (identity, progression, billing; the engine; the fleet) | `AGPL-3.0-only` | contributors sign the CLA, as well as the DCO sign-off |
| A tool, library, SDK, plugin, script or CI step (the edge) | `MIT` | DCO sign-off |
| Images, models, data, design, lore, agent cards | `CC0-1.0` | DCO sign-off |
| A mix of the above | one per path, in `REUSE.toml` | `LICENSES/` holds each text |

Copy the text from <https://spdx.org/licenses/> into `LICENSE` (or `LICENSES/<id>.txt` with `REUSE.toml`).
The names Numinia, Numen Games and Khepri are never licensed. If in doubt, ask Pablo before the first push.

## After "Use this template"

1. Choose the licence (table above) and commit it first.
2. Fill the `TODO` lines in `AGENTS.md` and write this README.
3. Settings → Advanced Security → Dependabot alerts: on. A template does not copy settings.
4. Give access to the GitHub Apps that work on it (Ursa's and `numinia-ci-puerta`).
5. Tell Ursa: she adds the repository to Hermes's list (`repos_numen.py`), its project and SYS-013.
