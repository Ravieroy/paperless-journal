## Uninstall Linux Applications 
Usually it is pretty simple to uninstall an application, using GUI tools like software managers. Sometimes some apps do not show up in GUI and hence we need to use [[Terminal]] to remove those applications. While the command to remove the application is simple, the exact name of the program needs to be known inorder to execute the command. 

```bash
apt-cache search ProgramName
```
Where, ProgramName is the partial or complete name of the program thats needs to be uninstalled. As an example, the following command will search for the program `okular`
```bash
apt-cache search okular
```
Once the correct name is known, simply issue the following command 
```bash
sudo apt purge ProgramName
```
or, 
```bash
sudo apt remove ProgramName
```
The [[Difference between purge and remove]] is that `purge` command removes the configuration files of the related program as well. 
