maps_toolkit
======

[![Pub Package](https://img.shields.io/pub/v/maps_toolkit.svg)](https://pub.dartlang.org/packages/maps_toolkit)
[![Build Status](https://travis-ci.org/kb0/maps_toolkit.svg?branch=master)](https://travis-ci.org/kb0/maps_toolkit)
[![Coverage Status](https://coveralls.io/repos/github/kb0/maps_toolkit/badge.svg?branch=master)](https://coveralls.io/github/kb0/maps_toolkit?branch=master)
[![GitHub Issues](https://img.shields.io/github/issues/kb0/maps_toolkit.svg?branch=master)](https://github.com/kb0/maps_toolkit/issues)
[![GitHub Forks](https://img.shields.io/github/forks/kb0/maps_toolkit.svg?branch=master)](https://github.com/kb0/maps_toolkit/network)
[![GitHub Stars](https://img.shields.io/github/stars/kb0/maps_toolkit.svg?branch=master)](https://github.com/kb0/maps_toolkit/stargazers)
[![GitHub License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://raw.githubusercontent.com/kb0/maps_toolkit/master/LICENSE)


A library for area, distance, heading measurements (spherical_util.dart if port from `android-maps-utils`).

## Getting Started

In your dart/flutter project add the dependency:

```
 dependencies:
   ...
   maps_toolkit: ^1.0.1+3
```

A simple usage example:

```dart
import 'package:maps_toolkit/maps_toolkit.dart';

main() {
  val distanceBetweenPoints = SphericalUtil.computeDistanceBetween(
    LatLng(51.5073509, -0.1277583),
    LatLng(48.856614, 2.3522219)
  );
}
```

## List of functions

* `SphericalUtil.computeArea` - calculate the area of a closed path on Earth.
* `SphericalUtil.computeDistanceBetween` - calculate the distance between two points, in meters.
* `SphericalUtil.computeHeading` - calculate the heading from one point to another point.
* `SphericalUtil.computeLength` - calculate the length of the given path, in meters, on Earth.
* `SphericalUtil.computeOffset` - calculate the point resulting from moving a distance from an origin in the specified heading (expressed in degrees clockwise from north).
* `SphericalUtil.computeOffsetOrigin` - calculate the location of origin when provided with a point destination, meters travelled and original heading.
* `SphericalUtil.computeSignedArea` - calculate the signed area of a closed path on Earth.
* `SphericalUtil.interpolate` - calculate the point which lies the given fraction of the way between the origin and the destination.

## Features and bugs

Please file feature requests and bugs at the [issue tracker][tracker].

[tracker]: https://github.com/kb0/maps_toolkit/issues
