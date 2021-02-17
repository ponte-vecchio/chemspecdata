`chemspecdata` is a LaTeX package that allows the user to easily label spectroscopic data, notably in the field of chemical sciences.

## Nuclear Magnetic Resonance (NMR) Spectroscopy
### Syntax

	\< nuclei >nmr[ < solvent > ]{ < peak > }

### Nuclei Types

`chemspecdata` entails not only the most commonly used isotopes (<sup>1</sup>H & <sup>13</sup>C) but also lesser known isotopes e.g. <sup>11</sup>B (geochemistry), <sup>15</sup>N (heterocycles, protein analysis), <sup>19</sup>F (radiochemistry) and <sup>31</sup>P (inorganic/organometallic chemistry).
- The process of corresponding the type of NMR with the name of the command should be intuitive -- proposed as the following:


	<sup>1</sup>H NMR : `\hnmr{ ... }`
	
	<sup>11</sup>B NMR : `\bnmr{ ... }`
	
	<sup>13</sup>C NMR : `\cnmr{ ... }`
	
	<sup>15</sup>N NMR : `\nnmr{ ... }`
	
	<sup>19</sup>F NMR : `\fnmr{ ... }`
	
	<sup>31</sup>P NMR : `\pnmr{ ... }`
	

### Solvents

`chemspecdata` allows for solvent shortcuts as well. List of common NMR solvents from [<i>Organometallics</i> 2010, 29, 9, 2176-2179](https://doi.org/10.1021/om100106e) were used and the outputs are mostly made to render as formulae as per [ACS guideline](https://pubsapp.acs.org/paragonplus/submission/acs_nmr_guidelines.pdf) unless inconvenient to do so (e.g. C<sub>6</sub>D<sub>6</sub> over benzene-<i>d</i><sub>6</sub>, but TFE-<i>d</i><sub>3</sub> over CF<sub>3</sub>CD<sub>2</sub>OD).

| < argument > | output |
| :--- | :--- |
| `chloroform`,`CDCl3` | CDCl<sub>3</sub> |
| `dcm`, `CD2Cl2` | CD<sub>2</sub>Cl<sub>2</sub> |
| `thf` | THF-d<sub>8</sub> | 
| `toluene` | toluene-<i>d</i><sub>8</sub> |
| `benzene`, `C6D6`| C<sub>6</sub>D<sub>6</sub> |
| `chlorobenzene`, `C6D5Cl` | C<sub>6</sub>D<sub>5</sub>Cl |
| `acetone` | (CD<sub>3</sub>)<sub>2</sub>CO |
| `dmso` | (CD<sub>3</sub>)<sub>2</sub>SO |
| `acetonitrile`, `MeCN` | CD<sub>3</sub>CN |
| `trifluoroethanol`, `tfe`  | TFE-<i>d</i><sub>3</sub> |
| `methanol` | CD<sub>3</sub>OD |
| `water` | D<sub>2</sub>O |

### Key Example

<sup>1</sup>H NMR ((CD<sub>3</sub>)<sub>2</sub>CO) δ 8.20 (br s, 1 H, PhOH) 7.14 (t, 1 H, *J* = 8.0 Hz, ArH para to PhOH) 6.89 (t, 1 H, *J* = 2.0 Hz,) 6.84 (d, 1 H, *J* = 8.0 Hz) 6.71 (dd, 1 H, *J* = 2.0, 8.0 Hz) 5.91 (br s, 1 H, NH) 4.68-4.72 (m, 1 H, CH) 4.50 (br s, 1 H, OH) 3.30–3.36 (m, 1 H, N–CH) 3.12–3.18 (m, 1 H, N–CH) 1.40 (s, 9 H, OC–CH<sub>3</sub>)
```tex
\hnmr[acetone]{%
    [8.20,{br s},1,,{PhOH}],
    [7.14,t,1,8.0,{ArH para to PhOH}],
    [6.89,t,1,2.0],
    [6.84,d,1,8.0],
    [6.71,dd,1,{2.0, 8.0}],
    [5.81,{br s},1,,{NH}],
    [{4.68--4.71},m,1,,{CH}],
    [4.50,{br s},1,,{OH}],
    [{3.30--3.36},m,1,,{N-CH}],
    [{3.12--3.18},m,1,,{N-CH}],
    [1.40,s,9,,\ce{OC-CH3}]
}%
```
## Infrared (IR) Spectroscopy

	TBD

## Mass Spectrometry (MS)

	TBD

## Ultraviolet-Visible Spectrophotometry (UV-Vis)

	TBD

## Melting Point Determination (m.p.)

	TBD

