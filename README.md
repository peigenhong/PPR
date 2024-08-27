# PPR
PowerShell Project Run with Windows Folder in sequence and Hierarchical structure
It was started in few years ago when doing the Grand Emperor upgrade to start/stop/change startup type/change service login password of the Advatange serviced.
Now with Mocha Adv975 upgraded, in the service part, I added create VBC cluster renew, dcim config, ADV report verification service control, also added to run SQL post upgraded scripts, configuration check and issue fixes
Added ADI Sync service jump start, Handpay migration.
the final goal is to have everything for a Advantage installation and upgraded integrated into the Project-Run structure.

Here is the first layer of the structure of the Project-Run:
1. SharedLib--contents all the internal/external scripts, application that needed for the project
2. MetaData--contents all the static information needed for the project, from property name, to server name, to application and service name, all in one json file
3. Logs folder to store all the logs generated during the process
4. Finally, the major part of the project run: StepRun, from here on, every steps can be addon in the sequence and hieracical structure
