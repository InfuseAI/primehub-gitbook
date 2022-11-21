# VSCode SSH Notebook Remotely

{% hint style="info" %}
This guide requires prerequisites of Notebook with enabled SSH Server feature and key-pair. Please go to SSH Server feature if it hasn't been set up yet.
{% endhint %}

### Steps

1.  Install the extension, [Remote - SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh) on VSCode.ssh

    <figure><img src="../../.gitbook/assets/ssh-remote-ext.png" alt=""><figcaption></figcaption></figure>
2.  Press `Cmd+Shift+p`, type `Remote-SSH:Connect to Host...` and run it.

    <figure><img src="../../.gitbook/assets/ssh-remote-cmd.png" alt=""><figcaption></figcaption></figure>
3.  Select `jupyter` from listed hosts, it will open a new VSCode window.

    <figure><img src="../../.gitbook/assets/ssh-remote-host.png" alt=""><figcaption></figcaption></figure>
4.  Once SSH succeeds, open file explorer and click `Open Folder`

    <figure><img src="../../.gitbook/assets/ssh-remote-folder.png" alt=""><figcaption></figcaption></figure>
5.  Open the folder, `/home/jovyan`.&#x20;

    <figure><img src="../../.gitbook/assets/ssh-remote-jovyan.png" alt=""><figcaption></figcaption></figure>
6.  It shows files from `/home/jovyan` of remote Notebook.

    <figure><img src="../../.gitbook/assets/ssh-remote-files.png" alt=""><figcaption></figcaption></figure>
