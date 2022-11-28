# Streamlit

Enterprise Applicable to Enterprise EditionCommunity Applicable to Community Edition

### Introduction

Streamlit turns data scripts into shareable web apps in minutes. All in Python. All for free. No front‑end experience required.

| Property         | Description                                                         |
| ---------------- | ------------------------------------------------------------------- |
| App Image        | [`infuseai/streamlit`](https://hub.docker.com/r/infuseai/streamlit) |
| Official Website | https://streamlit.io/                                               |

### Screenshots

### Usage

1. Create a Streamlit app
2. In the create page, fill the `FILE_PATH` variable. The server is run as the command `streamlit run ${FILE_PATH}`. You can fill a Streamlit python from:
   * Local file (e.g. `/project/<group-name>/path/to/your/file`)
   * Web URL (e.g. `https://raw.githubusercontent.com/streamlit/streamlit-example/master/streamlit_app.py`)
3. Open the Streamlit server you just created
4. You can see the Streamlit dashboard

### External Dependencies

You can manage external dependencies by adding:

* `requirements.txt` for Python dependencies managed by `pip`([docs](https://pip.pypa.io/en/stable/user\_guide/))
* `packages.txt` for Debian dependencies managed by `apt-get`([docs](https://linux.die.net/man/8/apt-get))

At the begin of statring, Streamlit will look for requirements files in the same directory of `FILE_PATH` and install external dependencies. Your Streamlit app is ready while the "You can now view your Streamlit app in your browser." shows up in the app logs.&#x20;

If there are a lots of dependencies, it may take some time to install while starting your app. Any change not related to dependencies should show up immediately. Remeber to restart your app after adding new dependencies.