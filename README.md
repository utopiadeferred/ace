
# bleh

| Parameter | Unit | Description |
|-----------|------|-------------|
| **Infooo** | | |
| name/shortName | text | Identification label for tire compound type |
| tyre_compound | text | Internal classification of tire compound type |
| **tyreData** | | |
| width | meters | Tire width |
| radius | meters | Overall tire radius from center to tread surface |
| rate | N/m | Vertical spring stiffness of the tire |
| damping | N·s/m | Vertical damping coefficient |
| angularInertia | kg·m² | Moment of inertia for rotational mass |
| rimRadius | meters | Wheel rim radius |
| radiusRaiseK | m/kN | Coefficient for how tire radius changes under load |
| treadHeightMM | mm | Height of the tread surface |
| treadConsumptionK | dimensionless | Tread wear rate coefficient |
| mass | kg | Mass of the tire |
| lateralFlexK | N/m | Sidewall lateral flex stiffness |
| lateralFlexC | N·s/m | Sidewall lateral flex damping |
| longitudinalFlexK | N/m | Tire longitudinal (fore-aft) flex stiffness |
| longitudinalFlexC | N·s/m | Tire longitudinal flex damping |
| explosionTemperature | °C | Temperature at which tire fails/bursts |
| blanketTemperature | °C | Starting temperature when using tire warmers |
| FlatSpotK | dimensionless | Flat spot development rate coefficient |
| contactCamber | degrees | Optimal camber angle for maximum contact patch |
| contactFlex | dimensionless | Contact patch flexibility coefficient |
| contactVerticalFlex | dimensionless | Vertical flex characteristic at contact patch |
| slipVibrationsThresholdMS | m/s | Slip speed threshold for vibration modeling |
| slipVibrationsScale | dimensionless | Amplitude scaling for slip vibrations |
| slipVibrationOmega | Hz | Frequency of slip vibrations |
| steerDamping | N·m·s/rad | Damping coefficient for steering inputs |
| steerDampingMz | N·m·s/rad | Self-aligning torque damping factor |
| **modelData** | | |
| Dy0 | dimensionless | Base lateral grip coefficient |
| Dx0 | dimensionless | Base longitudinal grip coefficient |
| lsExpY | dimensionless | Lateral slip exponent |
| lsExpX | dimensionless | Longitudinal slip exponent |
| Fz0 | N | Reference normal load for tire model |
| frictionLimitAngle | degrees | Maximum effective slip angle |
| flexGain | dimensionless | Tire flex influence on grip |
| cfXmult | dimensionless | Longitudinal force multiplier |
| brakeDXMod | dimensionless | Braking grip modification factor |
| combinedFactor | dimensionless | Combined lateral/longitudinal grip interaction |
| gripSlipFactor | dimensionless | Relation between slip and grip |
| wearCurve | path | Reference to wear model curve data |
| grainFactor | dimensionless | Surface grain development rate |
| contactWearIMO | dimensionless | Wear model influence on contact patch |
| relaxationLengthY | meters | Lateral force buildup distance |
| relaxationLengthX | meters | Longitudinal force buildup distance |
| mzTweakMult | dimensionless | Self-aligning torque multiplier |
| mzScale | dimensionless | Self-aligning torque magnitude scale |
| mzTrailNdSlipReduction | dimensionless | Self-aligning torque reduction with slip |
| mzTrailRemap | dimensionless | Self-aligning torque trail remapping |
| brushExponent | dimensionless | Brush model exponent for force calculation |
| **thermalData** | | |
| verticalSpringK | N/mm/°C | Thermal influence on vertical stiffness |
| verticalDampK | N·s/m/°C | Thermal influence on vertical damping |
| wearMult | 1/°C | Temperature influence on wear rate |
| frictionK | 1/°C | Temperature influence on friction |
| rollingK | N/°C | Temp influence on rolling resistance |
| rollingSurfaceK | N/°C | Surface temperature effect on rolling resistance |
| surfaceTransfer | W/(m²·K) | Heat transfer coefficient at surface |
| patchTransfer | W/(m²·K) | Heat transfer at contact patch |
| patchCoreTransfer | W/(m²·K) | Heat transfer: patch to core |
| internalCoreTransfer | W/(m²·K) | Internal heat transfer within core |
| coolFactor | W/(m²·K) | Base cooling coefficient |
| coolFactorRain | dimensionless | Cooling multiplier in wet conditions |
| coolFactorBase | dimensionless | Baseline cooling factor |
| coolFactorPhase | dimensionless | Cooling phase shift coefficient |
| coolFactorPhaseTref | °C | Reference temperature for cooling phase |
| grainGain | 1/°C | Thermal influence on grain development |
| grainGamma | 1/s | Grain decay rate |
| grainSlipAngleGain | 1/(°·s) | Slip angle influence on grain formation |
| grainSlipAngleGamma | 1/s | Grain decay from slip angle |
| grainSlipAngleThreshold | degrees | Slip angle threshold for grain formation |
| practicalTempSource | dimensionless | Temperature source weighting |
| brakeTransferFactor | dimensionless | Heat transfer from brakes to tire |
| thermalPerformanceCurve | path | Reference to thermal grip curve |
| contactIMO | dimensionless | Contact patch thermal model influence |
| TrefFrictionLimitAngle | °C | Reference temp for friction limit angle |
| frictionLimitAngleTSensitivity | deg/°C | Temperature sensitivity of friction limit angle |
| angularSpeedToSpeedK | dimensionless | Conversion factor for angular to linear speed |
| roadConduction | W/(m²·K) | Heat conduction to/from road surface |
| **pressureData** | | |
| pressureFlexGain | 1/PSI | Pressure influence on tire flexibility |
| rollingResistanceGain | dimensionless | Pressure effect on rolling resistance |
| rollingHeatGain | dimensionless | Heat generation from rolling at different pressures |
| gainD | 1/PSI | Pressure influence on grip coefficient D |
| idealPressure | PSI | Target pressure for optimal performance |
| pressureReference | PSI | Reference pressure for model parameters |
| pressureSpringGain | N/m/PSI | Pressure influence on spring rate |
| **camberData** | | |
| camberGain | dimensionless | Camber influence on grip |
| camberVerticalKRangeDeg | degrees | Camber range for vertical stiffness effect |
| camberVerticalKGain | dimensionless | Camber effect on vertical stiffness |
| dcamber0 | dimensionless | Camber effect parameter 0 |
| dcamber1 | 1/deg | Camber effect parameter 1 |
| **speedSensitivity** | | |
| ref_speed | m/s | Reference speed for grip calculations |
| temperature_speed_shift | °C | Temperature adjustment with speed |
| mu0T | dimensionless | Base friction coefficient at ref temperature |
| muTSensitivity | 1/°C | Temperature sensitivity of friction |
| muSpeedSensitivity | dimensionless | Speed sensitivity of friction |
| TrefMuT | °C | Reference temperature for friction model |
| **rollingResistance** | | |
| rr0 | N | Base rolling resistance force |
| rr1 | s/m | Speed coefficient for rolling resistance |
| rr_slip | N·s/m | Slip influence on rolling resistance |
| rrWearMult | dimensionless | Wear effect on rolling resistance |
| **grooveData (Groove Effects for Wet Conditions)** | | |
| grooveSAFactor | dimensionless | Groove effect on slip angle behavior |
| grooveSRFactor | dimensionless | Groove effect on slip ratio behavior |
| **Operating Settings** | | |
| pressure | PSI | Current operating pressure |
| init_data.width | mm | Nominal tire width |
| init_data.aspect_ratio | % | Height as percentage of width |
| init_data.diameter | inches | Wheel rim diameter |
| init_data.load_index | rating | Load capacity rating |
| init_data.pressure | PSI | Factory default pressure |
