# Engineering notes

## Engine layout
W16 = two VR8 units at 90°. Each VR8 has two banks 15° apart, so bank angles from vertical are ±37.5° and ±52.5°. All sixteen rods share one crankshaft. Real figures used: 7,993 cc, 86 × 86 mm bore and stroke, 64 valves, four turbochargers, 1,500 PS, 1,600 Nm from 2,000 to 6,000 rpm.

## Piston kinematics
Piston position along its bank axis, with crank radius r, rod length L and crank angle t:
`d = r·cos(t) + sqrt(L² − r²·sin²(t))`
Each rod rides on a real crank pin. The pin position in each bank's frame gives the angle t, so rod and piston motion are exact. Eight pins (two rods each) use the phase pattern 0, 180, 90, 270, 270, 90, 180, 0 degrees.

## Four-stroke cycle
Each cylinder's cycle angle is its crank angle plus an offset, wrapped to 720 degrees: power, exhaust, intake, compression. Valve lift is a half sine during its stroke, and cam lobes turn at half crank speed.

## Telemetry model
- Torque: ramps up to 1,600 Nm at 2,000 rpm, flat to 6,000 rpm, then tapers to about 1,572 Nm at 6,700 rpm.
- Power: `PS = Nm × rpm / 9549 × 1.35962`, which gives about 1,500 PS at 6,700 rpm.
- Boost: illustrative curve scaled from torque. It is not measured data.

## Known simplifications
- Geometry is procedural, not CAD. Firing order is approximate and plumbing is stylized.
- Model stroke-to-bore ratio is not 1:1 as on the real engine.
- Ignition glow marks pistons near top of stroke, not actual combustion.
- Turbo staging (about 3,800 rpm) is described but not simulated.
