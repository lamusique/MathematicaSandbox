
a = Slove[Mod[Log[x/440]/Log[2]  12, 12], x]
Note[x_] := Mod[Log2[x/440]/Log[2] 12, 12]

Plot[Mod[Log2[x/440] + 0.75, 1], {x, 110, 880}]

Note[x_] := Mod[Log2[x/440] + 0.75, 1]
Note[x_] := Mod[Log2[x/440] + 0.75, 1] 12
Note[x_] := Mod[Log2[x/440] + 0.75, 1] 12


C4
440 / 2^(9/12)
N[220 2^(1/4), 50]
c4 := 440 / 2^(9/12)

440/2^(9/12) * GoldenRatio

Note[c4 GoldenRatio^Range[0, 3]]

- - - - - - - - - - - - - - - - - - -

DiscretePlot[Note[440/2^(9/12) (x - 1)], {x, 1, 64},
 GridLines -> {Automatic, Range[1, 12]},
 Ticks -> {Automatic, Range[1, 12]}]

Plot[Note[440/2^(9/12) * GoldenRatio],{x,0,64}]

Show[DiscretePlot[Note[440/2^(9/12) (x - 1)], {x, 1, 64},
 GridLines -> {Automatic, Range[1, 12]},
 Ticks -> {Automatic, Range[1, 12]}], Plot[Note[440/2^(9/12) * GoldenRatio],{x,0,64}]]
Show[%, ImageSize -> Large]

Show[DiscretePlot[Note[440/2^(9/12) (x - 1)], {x, 1, 256},
 GridLines -> {Automatic, Range[1, 12]},
 Ticks -> {Automatic, Range[1, 12]}], Plot[Note[440/2^(9/12) * GoldenRatio],{x,0,256}]]

Show[%, PlotRange -> {{0, 256}, {8, 9}}]

Show[DiscretePlot[Note[440/2^(9/12) (x - 1)], {x, 1, 256},
 GridLines -> {Automatic, Range[1, 12]},
 Ticks -> {Automatic, Range[1, 12]}], Plot[Note[440/2^(9/12) * GoldenRatio],{x,0,256}], PlotRange -> {{0, 256}, {8, 9}}]

Show[DiscretePlot[Note[440/2^(9/12) (x - 1)], {x, 1, 256},
 GridLines -> {Automatic, Range[1, 12]},
 Ticks -> {Automatic, Range[1, 12]},PlotMarkers -> {"��"}], Plot[Note[440/2^(9/12) * GoldenRatio],{x,0,256}], PlotRange -> {{0, 256}, {8, 9}}]

Show[DiscretePlot[Note[440/2^(9/12) GoldenRatio^(x - 1)], {x, 1, 64},
 GridLines -> {Automatic, Range[1, 12]},
 Ticks -> {Automatic, Range[1, 12]}], Plot[Note[440/2^(9/12) * GoldenRatio],{x,0,256}]]


gr[x_] := N[440/2^(9/12) GoldenRatio^(x - 1), 20]
DiscretePlot[gr[x], {x, 0, 10}]

gr[Range[0, 10]]

MidiNote[d_] := 2^((d - 69)/12) 440

SuperCollider

{SinOsc.ar(161.69349168167505655, 0 , 0.5)}.play;
{SinOsc.ar(261.62556530059863468, 0 , 0.1)}.play;
{SinOsc.ar(423.31905698227369123, 0 , 0.1)}.play;
{SinOsc.ar(684.94462228287232591, 0 , 0.1)}.play;
{SinOsc.ar(1108.2636792651460171, 0 , 0.1)}.play;
{SinOsc.ar(1793.2083015480183431, 0 , 0.1)}.play;
{SinOsc.ar(2901.4719808131643602, 0 , 0.01)}.play;
{SinOsc.ar(4694.6802823611827033, 0 , 0.01)}.play;
{SinOsc.ar(7596.1522631743470634, 0 , 0.01)}.play;
{SinOsc.ar(12290.832545535529767, 0 , 0.01)}.play;
{SinOsc.ar(19886.984808709876830, 0 , 0.01)}.play;

Hz[f_] := 69 + 12 Log2[f/440]

- - - - - - - - - - - - - - - - - - -

Transform intervals


Surd[2,3] = 2^(1/3)

semitone up by golden ratio

MidiNote[85]/MidiNote[60]
Surd[MidiNote[85]/MidiNote[60],3]
