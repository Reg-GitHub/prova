# trm-server Setup

> The server-side component of TRM is identified as trm-server

## First install

The first install must be performed using [abapGit](https://abapgit.org/).

AbapGit is an open source git client for ABAP.

If you haven't installed it already, follow the official guide at [this link](https://docs.abapgit.org/user-guide/getting-started/install.html).

The minimum installation of abapGit requires the [standalone version](https://docs.abapgit.org/user-guide/getting-started/install.html#install-standalone-version).

Once abapGit installed, you can either install trm-server as an online or offline repository.

> If your system has [connection to Github](https://docs.abapgit.org/user-guide/setup/ssl-setup.html), it's recommended to install as an online repo

### Online repo

1. Run abapGit (standalone/developer)
2. On the repository list page, select "New Online"
3. Enter `https://github.com/RegestaItalia/trm-server` for the URL
4. Enter package name `ZTRM`
5. Select "Clone Online Repo"
6. Select "Pull"

### Offline repo

First download the latest release source code from
1. Direct link [https://github.com/RegestaItalia/trm-server/archive/refs/heads/main.zip](https://github.com/RegestaItalia/trm-server/archive/refs/heads/main.zip)
2. Open the [Github repo page](https://github.com/RegestaItalia/trm-server)
	1. Press the button "<> Code"
	2. Press "Download ZIP"
	
![image](https://github.com/RegestaItalia/trm-server/assets/87023474/bc654cff-25cf-4f9e-9b95-eb52465cff7a)

With the source code zip file saved on your computer
1. Run abapGit (standalone/developer)
2. On the repository list page, select "New Offline"
3. Enter repo name `trm-server` and package name `ZTRM`
1. Select "Create Offline Repo"
1. Select "Import <sup>zip</sup>"
1. Select the _trm-server-main.zip_ file
1. Select "Pull <sup>zip</sup>"


## Update

With trm-server already installed on your system, there are two ways to keep it up to date:

1. You may keep using [abapGit](https://abapgit.org/)
	- If it's an online repo, simply pull from the "main" branch
	- If it's an offline repo, download the "main" branch source code as "zip" from Github and import
2. You may use TRM Client and get from the Public Registry the latest release

Both method will assure you the latest version installed on your system.

## Check installation

To verify trm-server is installed properly:
1. Open transaction "SE80"
2. Open package "ZTRM"
3. Right click on the root package and press "Check > Package Check > Package Objects (Including Subpackages)"

This check should not give any errors.