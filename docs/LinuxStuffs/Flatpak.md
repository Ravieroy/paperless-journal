# Flatpak Software management
---

## Search Applications
In order to search for applications, one can use either [Flathub](https://flathub.org/home)website or use the following commands in [[Terminal]] after [[Setting up Flatpak]].
```bash
flatpak search keyWord 
```

## Install Applications 
Once the desired application is listed in the search results, we can use the **Application ID** to install the application. (*Remark: Application ID is to be used and not the name*)

![[flatpak_app_ID.png]]

```bash
flatpak install AppID
```
Then, few options will be provided for to install the application, i.e for user or system-wide. 

## Install Application from local *flatpakref* file
Download the flatpakref file and head over to the directory where it is located. Everything remains same as last.
```bash
flatpak install fileName
```

## List installed apps
To list all the installed Flatpak applications, 
```bash
flatpak list
```

## Run the application can be run like any other application by just searching for it. 
To run the application from [[Terminal]], 
```bash
flatpak run AppID
```

## Update applications
To update all the applications installed via Flatpak, use
```bash
flatpak update 
```

## Uninstall application 
To uninstall any application, 
```bash 
flatpak uninstall AppID
```

## Clean up unused libraries 
When an application is uninstalled, not all the dependencies are removed. To clear the unused libraries, 
```bash 
flatpak uninstall --unused
```

## Add other flatpak repo
The official repository is Flathub but we can add other repos as well by following command, 
```bash
flatpak remote-add repoName repoURL
```

## Remove flatpak repo
To remove the repo, 
```bash
flatpak remote-delete repoName
```

