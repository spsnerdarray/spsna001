# spsna001
CODESYS Projekt zur SPS Nerdarray Episode 20


PLC_PRG
```PASCAL
PROGRAM PLC_PRG
VAR
	
	counter : UINT;

	start : BOOL;
	stop : BOOL;
	reset : BOOL;
	run : BOOL;

END_VAR


IF start THEN
	start := FALSE;
	run := TRUE;
END_IF

IF stop THEN
	stop := FALSE;
	run := FALSE;
END_IF

IF reset THEN
	reset := FALSE;
	run := FALSE;
	counter := 0;	
END_IF

IF run THEN
	counter := counter + 1;
END_IF


END_PROGRAM
```
