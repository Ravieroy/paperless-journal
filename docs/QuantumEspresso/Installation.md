----
## Method 1 (Recommended) : Ubuntu or Fedora Linux 
### Ubuntu/Debian Based
```bash
sudo apt update && sudo apt upgrade
sudo apt install quantum-espresso
```

### Fedora or RHEL based 

```bash 
sudo dnf update 
sudo dnf install quantum-espresso
```

---
!!! note "PROS"
	1. Quick and Easy install process. 
	2. All serious works on DFT is done on Linux servers. 

!!! note "CONS"
	1. New unfamiliar OS if coming from Windows, thus learning curve is slightly steeper. 
	2. Lack of GUI and dependency on command line terminal.(IMO it is a pro in the long run)

!!! info "Important Links"
	1. [Quantum Espresso HomePage](https://www.quantum-espresso.org/)
	2. [Documentation for Installation from source(not needed)](https://www.quantum-espresso.org/Doc/user_guide/node1.html)
	3. [Hands On Example PDF](https://flex.phys.tohoku.ac.jp/QE/workshop_QE_2016/DFT-hands-on-nguyen.pdf)
	4. [Documentation](https://pranabdas.github.io/espresso/setup/pseudo-potential) 

!!! tip 
	The executables for the [[Quantum Espresso]] can be found in `/usr/bin`. We can check if executables like `pw.x` , `bands.x` are present in the directory or not. We can simply do `ls pw.x` and if there is no error then that file is present. We can also directly type `pw.x` in [[Terminal]] and it should not return any error. 

----
## Method 2 (Next best) : Windows Subsystem for Linux(WSL)

!!! note "PROS"
	1.  Familiar environment for Windows users with minor benefits of Linux.

!!! note "CONS"
	1. WSL is not optimised for this kind of tasks but is good enough for basic calculations. 
	2. Heavier tasks cannot be run. Period. 
	3. Same learning curve as Linux because it basically is Linux. 

---
## Method 3 : Native Windows
Follow the detail procedure as shown in [[QE_install_manual_en_win.pdf]] file. 

!!! note "PROS"
	1. Familiar environment for Windows users.(Thats it!!)

!!! note "CONS"
	1. Long procedure to set up the environment with moderately high chances of failure. 
	2. Windows is not optimised for this kind of tasks and hence will affect usability. 
	3. Heavier tasks cannot be run. Parallelization is a nightmare. 
	4. Not useful for long and serious calculations. 

Once the installation is successfully done we can go ahead and perform [[ SCF Calculation for Silicon]]

---
