Before we can run `bands` calculation, we need to perform [[SCF Calculation for Silicon]]. Next step is our band calculation (non-self consistent field) calculation. The `bands` calculation is _non self-consistent_ in the sense that it uses the ground state electron density, Hartree, exchange and correlation potentials determined in the previous step. In case of non self-consistent calculation, the `pw.x` program determines the Kohn-Sham eigenfunction and eigenvalues without updating Kohn-Sham Hamiltonian at every iteration. We need to specify the k-points for which we want to calculate the eigenvalues. We can also specify `nbnd`. Below is the input file for band calculation:
(We are using [[band.silicon.in]] file in this example)

```text
&CONTROL
  calculation = 'bands',

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

K_POINTS {crystal_b}
5
  0.0000 0.5000 0.0000 20  !L
  0.0000 0.0000 0.0000 30  !G
  -0.500 0.0000 -0.500 10  !X
  -0.375 0.2500 -0.375 30  !U
  0.0000 0.0000 0.0000 20  !G

```

To run the calculation, type in [[Terminal]]
```bash
mpirun -np 4 /usr/bin/pw.x < band.silicon.in > band.silicon.out
```

The bands are now calculated. We need some post processing in order to obtain the data in more usable manner. Input file for `bands.x`: ([[bands_pp.in]])
```text
&BANDS
  prefix = 'silicon'
  outdir = './'
  filband = 'si_bands.dat'
/
```

Then simply run, 
```bash
bands.x < bands_pp.in > bands_pp.out
```

Now this will create a lot of files among which we need `si_bands.dat.gnu` which we will use in `gnuplot` to plot the bandstructure. 

!!! tip 
	We can simply install `gnuplot` by typing in [[Terminal]] the following command
	`sudo apt install gnuplot`

## Plotting using `gnuplot`
`gnuplot` has several features, but we can simply do the following to get the plot quickly. Type `gnuplot` in [[Terminal]] and a new prompt will come up. We use the following commad to get the plot : 
```bash 
pl "si_bands.dat.gnu" w l lw 2
```

