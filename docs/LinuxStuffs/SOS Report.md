The sosreport command is **a tool that collects configuration and diagnostic information from a Red Hat Enterprise Linux system**. To run sosreport the sos package must be installed. The package is part of the default group and will be installed automatically on most systems. To check if `sos` package is installed type the command `rpm -qa |grep sos`. If the package is not already installed, we can install it from our [[Package Manager]] directly. 

Run following command with root permssion to create the sos report. Once completed, sosreport will generate a compressed a file under /tmp . The last step is to collect the `tar.xz` generated and attache to PMR/RTC for further analysis.

```bash
sos report
```
