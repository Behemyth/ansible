# ansible-core
Ansible collection for the Synodic organization

## Developer Setup

To install the required tools, you need [PDM](https://pdm-project.org/), a modern Python package and dependency manager.

Install PDM (recommended):

```bash
pipx install pdm
```

If you don't have pipx, install it with:

```bash
python3 -m pip install --user pipx
python3 -m pipx ensurepath
```

Or see the [official installation guide](https://pdm-project.org/latest/#installation) for more options.

Once PDM is installed, install project dependencies:

```bash
pdm install
```

This will also run a post-install script to set up system dependencies via Ansible.  
You may be prompted for sudo permissions.

If you need to re-run the system setup manually, you can use:

```bash
pdm run init
```

_Note: After setup, you may need to reload your shell or run `source /etc/profile.d/vagrant_wsl.sh` to enable the environment variable in your current session._

## Testing

To test everything, run

```base
pdm test
```