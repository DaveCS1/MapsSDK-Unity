# Changelog
All notable changes to the SDK NuGet package and it's supporting scripts will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and the SDK NuGet package adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## 0.1.5 - 2019-05-07
### Maps SDK
#### Fixed
- Networking performance improvements.

## 0.1.4 - 2019-04-30
### Maps SDK
#### Fixed
- Copyright TextMeshes are now positioned correctly when the map layout is not using the default dimensions.
- Cleaned up the ClusterMapPin editor UI to remove unnecessary properties.

## 0.1.3 - 2019-04-23
### Maps SDK
#### Fixed
- Regression in MapPin size when using real-world scale.

## 0.1.2 - 2019-04-22
### Maps SDK
#### Added
- Altitude can now be specified on MapPins.
- Maps SDK-related compnents will now have their help icons direct out to the relevant wiki doc page.
#### Fixed
- Custom Maps SDK component icons for the editor are now working again.
- MapPins childed to MapRenderer are positioned correctly in editor after script reloading.

## 0.1.1 - 2019-04-16 
### Maps SDK
#### Fixed
- Elevation terrain tiles will now fall back to lower LODs correctly.
- Seams between tiles should now be much less visible.

## 0.1.0 - 2019-04-09

### Maps SDK
#### Added
- MapRenderer component that handles streaming and rendering of 3D terrain data.
- MapPinLayer that allows for positioning GameObjects on the MapRenderer at a specified LatLon.
- Ability to cluster MapPins per MapPinLayer. This allows for efficiently rendering large data sets.
- Ability to animate the position and zoom level of the map via the SetMapScene API.
- MapLabelLayer for displaying city labels.
- Support for shadow casting and recieving of the map.
- Option to use a custom material for terrain.

### Supporting Scripts
#### Added
- Shader for rendering terrain with support for shadows, heightmap offsets, and clipping to the MapRenderer's dimensions.
- Shader for rendering side of map. Dynamically generates appropriate triangles by the geometry shader. Supports shadows.
- Script with helper functions to navigate the MapRenderer, e.g. panning and zooming.
- Script for animating map to the specified location and zoom level.
