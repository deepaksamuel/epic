# DRICH Simulation Parameters


Vessel Geometry: The DRICH vessel consists of a snout (conical front) and a tank (polycone (3 planes) with an inital cone and a cylinder). The sensorboxes are cylinders riding over the conical part of the tank and are merged with the tank solid in the geometry description

The snout houses the aerogel radiator, while the tank contains the majority of the detector components. 

The gas volume fills this vessel, and all other volumes are children.

Radiator: There are two radiators. The first radiator is composed of aerogel and a filter, separated by a small air gap. The aerogel thickness is 4.0 cm, and the filter thickness is 3.0 mm. The second radiator is a gas.

Sensors: The sensors are arranged in Photodetector Units (PDUs), each containing a 2x2 matrix of sensors. The sensors have a pixel size of 3.0 mm and a pitch of 3.2 mm.

Optical Properties: The mirror has a reflectivity of 90%, and the sensors have 100% efficiency for detecting photons.

Materials: The vessel is made of aluminum, the radiator uses aerogel and acrylic, and the gas inside the detector is C₂F₆.

| Variable Name          | Value            |
|------------------------|------------------|
| vesselZmin             | 198              |
| sensorboxRmin          | 108              |
| vesselLength           | 120              |
| sensorboxRmax          | 185              |
| vesselRmin0            | 8.62092          |
| sensorboxDphi          | 0.733038         |
| vesselRmin1            | 15.4779          |
| quartzwinLength        | 50               |
| vesselRmax0            | 90               |
| quartzwinRmin          | 108              |
| vesselRmax1            | 104.479          |
| quartzwinRmax          | 185              |
| vesselRmax2            | 180              |
| quartzwinDphi          | 0.733038         |
| snoutLength            | 20               |
| pssMat                 | AirOptical       |
| nSectors               | 6                |
| pssVis                 | DRICH_sensor_vis |
| wallThickness          | 1                |
| pssSurf                | SensorSurface_DRICH |
| windowThickness        | 0.3              |
| pssSide                | 2.56             |
| vesselMat              | Aluminum         |
| pssThickness           | 0.01             |
| gasvolMat              | C2F6_DRICH       |
| resinMat               | Epoxy            |
| quartzWindowMat        | QuartzOptical    |
| resinVis               | DRICH_vessel_vis |
| vesselVis              | DRICH_vessel_vis |
| resinSide              | 2.58             |
| gasvolVis              | DRICH_gas_vis    |
| resinThickness         | 0.135            |
| radiatorRmin           | 9.82092          |
| pduNumSensors          | 2                |
| radiatorRmax           | 88.8             |
| pduSensorGap           | 0.02             |
| radiatorPitch          | 0                |
| pduGap                 | 0.3              |
| radiatorFrontplane     | 0.3              |
| sensorSphRadius        | 110              |
| aerogelMat             | Aerogel_DRICH    |
| sensorSphCenterX       | 183.4            |
| aerogelVis             | DRICH_aerogel_vis |
| sensorSphCenterZ       | -59.6            |
| aerogelThickness       | 4                |
| sensorSphPatchPhiw     | 0.314159         |
| filterMat              | Acrylic_DRICH    |
| sensorSphPatchRmin     | 111              |
| filterVis              | DRICH_filter_vis |
| sensorSphPatchRmax     | 179              |
| filterThickness        | 0.3              |
| sensorSphPatchZmin     | 24               |
| airgapMat              | AirOptical       |
| airgapVis              | DRICH_gas_vis    |
| airgapThickness        | 0.001            |
| mirrorMat              | Acrylic_DRICH    |
| mirrorVis              | DRICH_mirror_vis |
| mirrorSurf             | MirrorSurface_DRICH |
| mirrorBackplane        | 1.3              |
| mirrorThickness        | 0.2              |
| mirrorRmin             | 15.4779          |
| mirrorRmax             | 176              |
| mirrorPhiw             | 1.03847          |
| focusTuneZ             | 6.15             |
| focusTuneX             | -7               |
| sensorboxLength        | 50               |
| OriginFront            | (0,0,-70)        |
| vesselPos              | (0,0,268)        |

# Geometries Overview

| Parameter                          | Value     |
|------------------------------------|-----------|
| OriginFront                        | (0,0,-70)       |
| vesselPos (origin)                 | (0,0,268)   |


## vesselSnout

| Parameter                          | Value     |
|------------------------------------|-----------|
| Half-length (z)                    | 10        |
| Inner radius at z = -half-length (rmin1) | 8.62092   |
| Outer radius at z = -half-length (rmax1) | 90        |
| Inner radius at z = +half-length (rmin2) | 9.76375   |
| Outer radius at z = +half-length (rmax2) | 104.479   |

## gasvolSnout

| Parameter                          | Value     |
|------------------------------------|-----------|
| Half-length (z)                    | 10        |
| Inner radius at z = -half-length (rmin1) | 9.62092   |
| Outer radius at z = -half-length (rmax1) | 89        |
| Inner radius at z = +half-length (rmin2) | 10.7466   |
| Outer radius at z = +half-length (rmax2) | 103.696   |

## vesselTank

| Parameter                          | Value     |
|------------------------------------|-----------|
| Phi range                          | 0 to 6.28319 |
| Inner radii (rmin):                | 9.76375, 11.478, 15.4779 |
| Outer radii (rmax):                | 104.479, 180, 180 |
| Z positions:                       | -50, -20, 50 |

## gasvolTank

| Parameter                          | Value     |
|------------------------------------|-----------|
| Phi range                          | 0 to 6.28319 |
| Inner radii (rmin):                | 10.7466, 12.466, 16.4779 |
| Outer radii (rmax):                | 103.696, 179, 179 |
| Z positions:                       | -49.7, -19.7, 49.7 |

## vesselSensorboxTube

| Parameter                          | Value     |
|------------------------------------|-----------|
| Inner radius (rmin)                | 108       |
| Outer radius (rmax)                | 185       |
| Half-length (z)                    | 25        |
| Phi start                          | -0.366519 |
| Phi end                            | 0.366519  |

## gasvolSensorboxTube

| Parameter                          | Value     |
|------------------------------------|-----------|
| Inner radius (rmin)                | 109       |
| Outer radius (rmax)                | 184       |
| Half-length (z)                    | 25        |
| Phi start                          | -0.361114 |
| Phi end                            | 0.361114  |

## vesselUnion

| Parameter                          | Value     |
|------------------------------------|-----------|
| First solid                        | vesselTank |
| Second solid                       | vesselSnout |
| Position of second solid           | Position(0., 0., -60) |

## gasvolUnion

| Parameter                          | Value     |
|------------------------------------|-----------|
| First solid                        | gasvolTank |
| Second solid                       | gasvolSnout |
| Position of second solid           | Position(0., 0., -59.7) |

## Sensorbox Unions

| Sector | Rotation | Position of vesselSensorboxTube | Position of gasvolSensorboxTube |
|--------|----------|---------------------------------|---------------------------------|
| 0      | 0.523599 | Position(0., 0., -34.7)         | Position(0., 0., -34.7)         |
| 1      | 1.5708   | Position(0., 0., -34.7)         | Position(0., 0., -34.7)         |
| 2      | 2.61799  | Position(0., 0., -34.7)         | Position(0., 0., -34.7)         |
| 3      | 3.66519  | Position(0., 0., -34.7)         | Position(0., 0., -34.7)         |
| 4      | 4.71239  | Position(0., 0., -34.7)         | Position(0., 0., -34.7)         |
| 5      | 5.75959  | Position(0., 0., -34.7)         | Position(0., 0., -34.7)         |

# Additional Quartz Window Parameters

| Constant Name                      | Value            | Description                                      |
|------------------------------------|------------------|--------------------------------------------------|
| DRICH_quartzwindow_thickness       | 0.05*cm          | Thickness of quartz window                       |
| DRICH_quartzwindow_rmin            | 1042*mm          | Lower radial limit of quartz window              |
| DRICH_quartzwindow_rmax            | 1790*mm          | Upper radial limit of quartz window              |
| DRICH_quartzwindow_zmin            | 2259*mm          | Z-position at lower radial limit of quartz window |
| DRICH_quartzwindow_zmax            | 2545*mm          | Z-position at upper radial limit of quartz window |
| DRICH_quartzwindow_dphi            | 42*degree        | Azimuthal width of quartz window (same as sensor box for now) |
| material            | QuartzOptical        |  |