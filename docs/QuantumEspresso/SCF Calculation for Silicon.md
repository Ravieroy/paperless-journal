Once the [[Installation]] for [[Quantum Espresso]] is done, we can go ahead and perform some basic calculations. Here we will do that for Silicon. 

## Self consistent field calculation for silicon
### Input Files 
Inorder to perform the SCF we need information about Silicon which is provided in `pw.scf.silicon.in` ([[pw.scf.silicon.in]]) whose content is as following :

!!! tip 
	The naming convention is like this ; 
	
	*pw*  : plane waves, 
	
	*scf*  : the file is to be used for scf calculation only,
	 
	*silicon* : name of the material
	
	*in* : input file 

```text
&CONTROL
  calculation = 'scf',

  prefix = 'silicon',

  outdir = './'

  pseudo_dir = './'

  verbosity = 'high'
/

&SYSTEM
  ibrav =  2,

  celldm(1) = 10.26,

  nat =  2,

  ntyp = 1,

  ecutwfc = 30

  nbnd = 8
/

&ELECTRONS
  mixing_beta = 0.6
/

ATOMIC_SPECIES
  Si 28.086 Si.pbe-n-kjpaw_psl.1.0.0.UPF

ATOMIC_POSITIONS (alat)
  Si 0.0 0.0 0.0
  Si 0.25 0.25 0.25

K_POINTS (automatic)
  6 6 6 0 0 0
```

We also need pseudopotential for Silicon, which can be downloaded from [here](http://pseudopotentials.quantum-espresso.org/legacy_tables) and kept in the working directory. Make sure that the name of the pesudopotential matches with the name in input file. (We have used [[Si.pbe-n-kjpaw_psl.1.0.0.UPF]] in this exampl)
```text
ATOMIC_SPECIES
  Si 28.086 Si.pbe-n-kjpaw_psl.1.0.0.UPF
```

Now we can go ahead and start the SCF calculation by simply typing this in [[Terminal]]
```bash 
pw.x < pw.scf.silicon.in > pw.scf.silicon.out
```

Or for parallel calculation, we can do 
```bash
mpirun -np 4 pw.x -inp pw.scf.silicon.in > pw.scf.silicon.out
```

!!! note 
	The executables should already be in the PATH but if the above command throws error, then we can add full path to the executable to run the code.
	`mpirun -np 4 /usr/bin/pw.x < pw.scf.silicon.in > pw.scf.silicon.out`

Now let’s look at the output file `pw.scf.silicon.out` and see how the convergence is reached:
```bash
grep -e 'total energy' -e estimate pw.scf.silicon.out
```

Once SCF is converged, we can do [[Band structure calculation for Silicon ]]. 