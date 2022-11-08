# FH-remote-install README

Basically, FH-remote-install will automate, for every feedhandler project in the active workspace the following:

* Compilation in test server
* Copy production instance of the feedhanler based on the choise of the user
* Upgarde the dev compiled version using the automatic steps of Quantflow

## Requirements

sshpass is required to use this extension.

## Extension Settings

Once the plugin installed, you need to check if default setting are good. (Cltr+,)

![Settings](images/1settings.png)

## How does It work

Open **Command Patette** (Cltr+Shift+P): and tape <span style="color:green">"Configure Remote Install"</span>

![Configure Remote Install](images/2configureRemoteInstall.gif)

If every thing is going well, you will see the following info message:

![info](images/3info.png)

Check that in every project in the active workspace there is a new file created : .<span style="color:green">vscode/tasks.json</span>

![check tasks.json](images/3checktasks.gif)

Now if you tape **Terminal->Run Build Task**(Cltr+Alt+B),you will see diffrents build for every project.

If we click on cme_mdp3, thebuild is lauched as follow and thecompilation began:

![compilation](images/4compilation.gif)

Once the compilation is done, A new list of production server is displayed,

In this demo, we choose the instance CME_CBOT_FUTURES_HW_SPEC:aurcme-fh101102

![choose production server ](images/5chooseprodserver.gif)

A copy of the production instance is installed on the rnd server.

![Install](images/6install.gif)

Now steps of automatic Quantflow will be applied.

![Apply QF](images/7applyQF.gif)

![Apply QF](images/71applyQF.gif)

-----------------------------------------------------------------------------------------------------------
