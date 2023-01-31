# Notebook Tips

### Install Custom Software

Users are able to run `sudo apt <command>` in a terminal of a Jupyter or `!sudo apt <command> --assume-yes` in a Jupyter Notebook to install required softwares in the environment.

### Notebook Logs

Notebooks, sometimes, are failed to spawn or run into troubles because user programs/environments. Now users are able to investigate failures and shoot troubles from logs of [Notebook Logs](./#notebook-logs).

### Safe Mode

When a user's jupyter pod cannot be launched successfully, try to launch the Notebook under [Safe Mode](advanced-settings.md#safe-mode) for _**troubleshooting**_. If the Notebook can be launched under Safe Mode, which implies two possible causes

* User's home folder `/home/jovyan`is full so that jupyter is not able to write its own files successfully.
* There is something wrong with packages which are installed by users causing problems during Jupyter initialization.

Under Safe Mode, try to

* Clean up home folder to make space for Jupyter.
* Uninstall installed packages one-by-one to find out which package interrupt Jupyter initialization.
