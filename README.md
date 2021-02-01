`chemspecdata` is a LaTeX package that allows the user to easily label spectroscopic data, notably in the field of chemical sciences.

## Functionality (Planned)
### Nuclear Magnetic Resonance (NMR) Spectroscopy
#### Overview

- The commands for NMR should entail not only the most commonly used isotopes (<sup>1</sup>H & <sup>13</sup>C) but also lesser known isotopes e.g. <sup>11</sup>B (geochemistry), <sup>15</sup>N (heterocycles, protein analysis), <sup>19</sup>F (radiochemistry) and <sup>31</sup>P (inorganic/organometallic chemistry).

- The process of corresponding the type of NMR with the name of the command should be intuitive -- proposed as the following:

	<sup>1</sup>H NMR : `\hnmr{<arg>}`
	
	<sup>11</sup>B NMR : `\bnmr{<arg>}`
	
	<sup>13</sup>C NMR : `\cnmr{<arg>}`
	
	<sup>15</sup>N NMR : `\nnmr{<arg>}`
	
	<sup>19</sup>F NMR : `\fnmr{<arg>}`
	
	<sup>31</sup>P NMR : `\pnmr{<arg>}`
	
	TBD
#### Key Example


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
### Infrared (IR) Spectroscopy

	TBD

### Mass Spectrometry (MS)

	TBD

### Ultraviolet-Visible Spectrophotometry (UV-Vis)

	TBD

### Melting Point Determination (m.p.)

	TBD

