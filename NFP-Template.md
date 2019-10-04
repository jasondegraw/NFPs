# NFP: Template #

## Justification for New Feature ##
TBD

## Overview ##
TBD

## Approach ##
TBD

## Engineering Reference ##
TBD

## I/O Reference ##
Describe the IO changes:

```
AirflowNetwork:MultiZone:Zone,
      \min-fields 8
      \extensible:1
      \memo This object is used to simultaneously control a thermal zone's window and door openings,
      \memo both exterior and interior.
  A1, \field Zone Name
      \required-field
      \reference AirFlowNetworkMultizoneZones
      \type object-list
      \object-list ZoneNames
      \note Enter the zone name where ventilation control is required.

  ...

  A6, \field Occupant Ventilation Control Name
      \type object-list
      \object-list AirflowNetworkOccupantVentilationControlNames
      \note Enter the name where Occupancy Ventilation Control is required.
  N7, \field Source Sink Muliplier
      \type real
      \default 1.0
      \note Multiplier to be applied to sources and sinks
  A7, \field Contaminant Source Sink 1
      \begin-extensible
      \type object-list
      \object-list AirflowNetworkMaterialSourceSinks
  A8, \field Contaminant Source Sink 2
      \type object-list
      \object-list AirflowNetworkMaterialSourceSinks
  ...
```

## Output Details ##
TBD

## Example File and Transition Changes ##
TBD

## Discussion and Comments
TBD

## References ##
Urbuddy, Ima N., and That O. Guy. "I'm not your buddy, guy" 2014. Report #?.
