# geom

This crate contains primitive types used by A/B Street and osm2streets. There
are many assumptions (and bugs) driven by these use cases, so it's not
recommended to depend on this for new work. The crate both wraps
[georust](https://github.com/georust/geo) and adds its own (usually buggy)
algorithms. The long-term fate of this crate of this library is unknown;
ideally it's replaced entirely by georust or becomes a very thin wrapper on it.

## Contents

Many of the types are geometric: `Pt2D`, `Ring`, `Distance`, `Line`,
`InfiniteLine`, `FindClosest`, `Circle`, `Angle`, `LonLat`, `Bounds`,
`GPSBounds`, `PolyLine`, `Polygon`, `Triangle`.

Some involve time: `Time`, `Duration`, `Speed`.

And there's also a `Percent` wrapper and a `Histogram`.
