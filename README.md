# Tom's VCV Racks

- Racks that start with `midi_` require a midi source (like a keyboard or daw or tracker or something)
- Racks that start with `seq_` might require you to hit a 'run' button

`.vcv` rack savestate files seem like JSON. I was able to extract the instruments via:
```
$ jq '.modules[].plugin' *.vcv | sort | uniq
```

"AudibleInstruments"
"Befaco"
"Core"
"ESeries"
"Fundamental"
"RJModules"
"VCV-PulseMatrix"
