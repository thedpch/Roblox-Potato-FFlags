# Roblox Optimization (and visual) FFlags v7.3 ![](https://pixels.crd.co/assets/images/gallery13/4bae341f.gif)

## Potato Flags

Forces Direct3D11 (better performance on newer pcs)

```json
{
  "FFlagDebugGraphicsDisableDirect3D11": false,
  "FFlagDebugGraphicsPreferD3D11": true,
  "FFlagDebugGraphicsPreferD3D11FL10": false
}
```

Forces Direct3D10 (better performance on older PCs)

```json
{
  "FFlagDebugGraphicsDisableDirect3D11": false,
  "FFlagDebugGraphicsPreferD3D11": false,
  "FFlagDebugGraphicsPreferD3D11FL10": true,
  "FFlagGraphicsEnableD3D10Compute": true
}
```

Forces Vulkan (can crash)

```json
{
  "FFlagDebugGraphicsDisableVulkan": false,
  "FFlagDebugGraphicsDisableVulkan11": false,
  "FFlagDebugGraphicsPreferVulkan": true,
  "FFlagRenderVulkanFixMinimizeWindow": true
}
```

Forces Metal (only for macOS (?) and should give perf boost?? idk)

```json
{
  "FFlagDebugGraphicsPreferMetal": true
}
```

Forces Voxel lightning

```json
{
  "DFFlagDebugRenderForceTechnologyVoxel": true
}
```

Disables terrain grass (?)

```json
{
  "FIntFRMMinGrassDistance": 0,
  "FIntFRMMaxGrassDistance": 0,
  "FIntRenderGrassDetailStrands": 0,
  "FintRenderGrassHeightScaler": 0
}
```

Breaks Voxel shadows (only works w/ voxel lightning)

```json
{
  "DFFlagDebugPauseVoxelizer": true
}
```

Makes Roblox at high res. lower quality

```json
{
  "DFFlagDisableDPIScale": false
}
```

Disables textures (doesn't give perf boost, only visual)

```json
{
  "FStringPartTexturePackTablePre2022": "{\"glass\":{\"ids\":[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\"color\":[254,254,254,7]}}",
  "FStringPartTexturePackTable2022": "{\"glass\":{\"ids\":[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\"color\":[254,254,254,7]}}",
  "FStringTerrainMaterialTablePre2022": "",
  "FStringTerrainMaterialTable2022": ""
}
```

Disables textures and breaks glass (alternative for one above)

```json
{
  "FStringPartTexturePackTablePre2022": "",
  "FStringPartTexturePackTable2022": "",
  "FStringTerrainMaterialTablePre2022": "",
  "FStringTerrainMaterialTable2022": ""
}
```

Disables player shadows

```json
{
  "FIntRenderShadowIntensity": 0
}
```

Disables some effects (like sunrays)

```json
{
  "FFlagDisablePostFx": true
}
```

Disables antialiasing

```json
{
  "FIntDebugForceMSAASamples": 0
}
```

Makes textures low quality

```json
{
  "DFFlagTextureQualityOverrideEnabled": true,
  "DFIntTextureQualityOverride": 0
}
```

Lowers model polygons from far

```json
{
  "DFIntCSGLevelOfDetailSwitchingDistance": 0,
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": 0,
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": 0,
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": 0
}
```

Limits light updates

```json
{
  "FIntRenderLocalLightUpdatesMax": 1,
  "FIntRenderLocalLightUpdatesMin": 1
}
```

Enables gray sky w/ no clouds

```json
{
  "FFlagDebugSkyGray": true
}
```

Disables Selfview

```json
{
  "FFlagCoreGuiTypeSelfViewPresent": false
}
```

Forces graphics quality to 1 (while being able to change render distance!)

```json
{
  "DFIntDebugFRMQualityLevelOverride": 1
}
```

Enable Hyperthreading

```json
{
 "FFlagRenderCheckThreading": "True"
}
```

Removes most textures of other players
```json
{
  "DFIntTextureCompositorActiveJobs": 0
}
```

## How to add FFlags to this list

Please do not open an issue, instead make a pull request and add the FFlag to the correct section, with the correct format and below the latest FFlag
```json
{
  "Flag1": "Value",
  "Flag2" : 23
}
```




{
  "FFlagHandleAltEnterFullscreenManually": "False",
  "FLogNetwork": "7",
  "DFIntTaskSchedulerTargetFps": "360",
  "DFLogHttpTraceLight": "0",
  "FFlagEnableMenuControlsABTest": "False",
  "FFlagFixGraphicsQuality": "True",
  "FFlagEnableInGameMenuModernization": "False",
  "FFlagDisableNewIGMinDUA": "True",
  "DFIntCanHideGuiGroupId": "32380007",
  "FFlagEnableInGameMenuControls": "False",
  "FFlagEnableMenuModernizationABTest": "False",
  "FStringPartTexturePackTable2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7546645012\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[255,255,255,255]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7546650097\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[204,201,200,232]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7546652947\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[212,200,187,250]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7546653951\u0022,\u0022rbxassetid://7546654144\u0022],\u0022color\u0022:[208,208,208,255]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547162198\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[170,170,170,255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547101130\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[105,104,102,244]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547304948\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[254,254,254,7]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547164710\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[113,113,113,255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547169285\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[165,165,159,255]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547171356\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[255,255,255,255]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547177270\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[199,199,199,255]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547288171\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[199,199,199,255]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547291361\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[208,208,208,255]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547184629\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[159,119,95,200]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547295153\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[220,220,220,255]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547298114\u0022,\u0022rbxassetid://7547298323\u0022],\u0022color\u0022:[193,193,193,255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547303225\u0022,\u0022rbxassetid://7547298786\u0022],\u0022color\u0022:[227,227,227,255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547332968\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[212,209,203,255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873267379\u0022,\u0022rbxassetid://9438410548\u0022],\u0022color\u0022:[123,123,123,234]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873270487\u0022,\u0022rbxassetid://9438413638\u0022],\u0022color\u0022:[154,154,153,238]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9438582231\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[74,78,80,156]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9438851661\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[226,229,229,243]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9439044431\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[114,114,112,240]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873288083\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[121,117,113,234]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873289812\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[235,234,230,250]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873319819\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[130,130,130,252]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873322398\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[142,142,144,236]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873515198\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[154,154,154,248]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9439566986\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[220,220,221,255]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873521380\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[174,171,169,246]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9439632387\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[218,218,218,255]}}",
  "FFlagEnableMenuModernizationABTest2": "False",
  "FFlagEnableV3MenuABTest3": "False",
  "DFFlagDisableDPIScale": "True",
  "FFlagDebugForceFutureIsBrightPhase3": "True",
  "FFlagEnableInGameMenuChrome": "true",
  "FFlagEnableAccessibilitySettingsAPIV2": "True",
  "DFIntLightstepHTTPTransportHundredthsPercent2": "0",
  "FFlagDebugDisableTelemetryV2Event": "True",
  "FFlagEnableAccessibilitySettingsEffectsInCoreScripts2": "True",
  "DFStringRobloxAnalyticsURL": "null",
  "DFIntS2PhysicsSenderRate": "250",
  "FFlagCoreGuiTypeSelfViewPresent": "False",
  "DFIntTextureQualityOverride": "3",
  "FFlagInGameMenuV1FullScreenTitleBar": "False",
  "FFlagDebugDisableTelemetryEphemeralStat": "True",
  "FFlagDebugDisableTelemetryPoint": "True",
  "DFStringCrashUploadToBacktraceBaseUrl": "null",
  "FStringGamesUrlPath": "/games/",
  "DFFlagBaseNetworkMetrics": "False",
  "DFStringTelemetryV2Url": "null",
  "GoogleAnalyticsAccountPropertyIDPlayer": "null",
  "FIntCameraMaxZoomDistance": "99999",
  "DFStringAltTelegrafHTTPTransportUrl": "null",
  "FFlagVoiceBetaBadge": "False",
  "FFlagCommitToGraphicsQualityFix": "True",
  "FStringCoreScriptBacktraceErrorUploadToken": "null",
  "FFlagNewLightAttenuation": "False",
  "DFStringLightstepHTTPTransportUrlPath": "null",
  "FFlagEnableInGameMenuChromeABTest": "True",
  "DFStringLightstepToken": "null",
  "DFFlagEnableLightstepReporting2": "False",
  "DFStringLightstepHTTPTransportUrlHost": "null",
  "FFlagEnableInGameMenuV3": "False",
  "FFlagDebugDisableTelemetryEphemeralCounter": "True",
  "FFlagAdServiceEnabled": "False",
  "DFStringTelegrafHTTPTransportUrl": "null",
  "FFlagCloudsReflectOnWater": "True",
  "FFlagEnableAccessibilitySettingsInExperienceMenu2": "True",
  "FFlagPreloadAllFonts": "True",
  "DFFlagBrowserTrackerIdTelemetryEnabled": "False",
  "DFStringCrashUploadToBacktraceWindowsPlayerToken": "null",
  "FFlagDebugDisableTelemetryEventIngest": "True",
  "DFStringAltHttpPointsReporterUrl": "null",
  "DFFlagDebugPerfMode": "True",
  "FFlagFastGPULightCulling3": "True",
  "DFIntClientLightingTechnologyChangedTelemetryHundredthsPercent": "0",
  "DFStringHttpPointsReporterUrl": "null",
  "FFlagDebugDisableTelemetryV2Counter": "True",
  "FFlagEnableAccessibilitySettingsEffectsInExperienceChat": "True",
  "FFlagDebugDisableTelemetryV2Stat": "True",
  "GoogleAnalyticsAccountPropertyID": "null",
  "DFStringCrashUploadToBacktraceMacPlayerToken": "null",
  "FFlagLuaAppSystemBar": "
 
