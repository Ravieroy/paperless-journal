[Source](https://itsfoss.com/how-to-remove-or-delete-ppas-quick-tip/)

# Remove or Delete PPA in Ubuntu/Debian
## Method 1
### From the source list in the [[Terminal]]
!!! warning
*Be conscious while using this method as it requires the use of sudo. It works fine*

You can remove the PPA from the sources list where these PPAs are stored. PPA repositories are store in the form of PPA_Name.list.

Use the following command to see all the PPAs added in your system:
`ls /etc/apt/sources.list.d`

Look for your desire PPA here and then remove the .list file associated with the PPA using the following command:

`sudo rm -i /etc/apt/sources.list.d/PPA_Name.list`

The `-i` option with rm command asks before removing a file. Consider this a safety check.

----
