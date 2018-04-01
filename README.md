# Tom's VCV Racks

- Racks that start with `midi_` require a midi source (like a keyboard or daw or tracker or something)
- Racks that start with `seq_` might require you to hit a 'run' button

`.vcv` rack savestate files seem like JSON. I was able to extract the instruments via:
```
$ jq '.modules[].plugin' *.vcv | sort | uniq
```

## Module Summary
```
AS
AudibleInstruments
Befaco
Core
ESeries
Fundamental
JW-Modules
RJModules
VCV-PulseMatrix
tnorris-BostonBrightonModules
```

## Module by Patch

```
Modules in midi_kwah.vcv
AudibleInstruments
Core
ESeries
Fundamental
RJModules
VCV-PulseMatrix

Modules in scope_twisty.vcv
AS
Fundamental

Modules in seq_homes.vcv
AS
AudibleInstruments
Befaco
Core
Fundamental
JW-Modules
RJModules
VCV-PulseMatrix
tnorris-BostonBrightonModules

Modules in seq_kicks.vcv
AudibleInstruments
Befaco
Core
Fundamental
RJModules
VCV-PulseMatrix

Modules in seq_shifty-pulse-matrix.vcv
AudibleInstruments
Befaco
Core
Fundamental
RJModules
VCV-PulseMatrix

Modules in seq_split-drums.vcv
AudibleInstruments
Befaco
Core
Fundamental
RJModules
VCV-PulseMatrix
tnorris-BostonBrightonModules

Modules in seq_untitled.vcv
AudibleInstruments
Befaco
Core
Fundamental
RJModules

Modules in seq_wubjams.vcv
AudibleInstruments
Befaco
Core
Fundamental
RJModules
```
