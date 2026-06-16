# Valhalla (valhalla)

Valhalla is an open-source routing engine and library suite for OpenStreetMap data. It provides turn-by-turn navigation, isochrone computation, time-distance matrix analysis, map matching, elevation sampling, optimized routing (TSP), and graph expansion via a REST API. Valhalla supports multiple travel modes including auto, bicycle, pedestrian, transit, truck, motorcycle, and motor scooter. It uses a tiled hierarchical data structure for efficient offline routing and regional extracts, with dynamic costing via a plugin architecture.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/valhalla/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/valhalla/refs/heads/main/apis.yml)

## Tags

- Routing
- Navigation
- OpenStreetMap
- Mapping
- Geospatial
- Directions
- Isochrones
- Travel
- Transportation
- Open Source

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### Valhalla Route API

Turn-by-turn routing service that guides users between two or more points by car, bike, foot, and multimodal combinations. Supports multiple costing models including auto, bicycle, pedestrian, truck, motorcycle, motor scooter, taxi, and multimodal (pedestrian + transit).

- **Human URL:** [https://valhalla.github.io/valhalla/api/turn-by-turn/api-reference/](https://valhalla.github.io/valhalla/api/turn-by-turn/api-reference/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Routing
- Navigation
- Turn-by-Turn
- Directions

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/api/turn-by-turn/api-reference/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Valhalla Optimized Route API

Solves the Travelling Salesman Problem (TSP) by computing an optimized path through multiple input locations. The service reorders intermediate waypoints for maximum efficiency, starting at the first and ending at the last location. Supports auto, bicycle, and pedestrian costing models.

- **Human URL:** [https://valhalla.github.io/valhalla/api/optimized/api-reference/](https://valhalla.github.io/valhalla/api/optimized/api-reference/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Routing
- Optimization
- TSP
- Travelling Salesman

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/api/optimized/api-reference/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Valhalla Matrix API

Computes time and distance matrices between sets of origins and destinations. Supports one-to-many, many-to-one, and many-to-many queries. Returns null for unreachable location pairs. Useful for logistics, delivery optimization, and accessibility analysis.

- **Human URL:** [https://valhalla.github.io/valhalla/api/matrix/api-reference/](https://valhalla.github.io/valhalla/api/matrix/api-reference/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Matrix
- Time-Distance
- Logistics
- Accessibility

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/api/matrix/api-reference/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Valhalla Isochrone API

Calculates isochrones (reachable areas within a given time or distance) and isodistances from one or more locations. Returns GeoJSON polygons or lines. Supports auto, bicycle, pedestrian, and multimodal costing. Output can also be returned as GeoTIFF raster format.

- **Human URL:** [https://valhalla.github.io/valhalla/api/isochrone/api-reference/](https://valhalla.github.io/valhalla/api/isochrone/api-reference/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Isochrones
- Reachability
- GeoJSON
- Accessibility

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/api/isochrone/api-reference/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Valhalla Map Matching API

Matches GPS traces and coordinate sequences to the road network mapped in OpenStreetMap. Provides two modes: trace_route (turns a GPS trace into a route with narrative instructions) and trace_attributes (returns edge and node attributes matched along the trace). All requests should use HTTP POST.

- **Human URL:** [https://valhalla.github.io/valhalla/api/map-matching/api-reference/](https://valhalla.github.io/valhalla/api/map-matching/api-reference/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Map Matching
- GPS
- Trace
- Navigation

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/api/map-matching/api-reference/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Valhalla Elevation API

Returns elevation data along a path or at specified locations. Accepts coordinate arrays or encoded polylines and returns height values in meters or feet. Supports cumulative distance ranges and configurable resampling intervals along the path.

- **Human URL:** [https://valhalla.github.io/valhalla/api/elevation/api-reference/](https://valhalla.github.io/valhalla/api/elevation/api-reference/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Elevation
- Terrain
- Height
- Geospatial

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/api/elevation/api-reference/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Valhalla Expansion API

Returns a GeoJSON representation of the routing graph traversal from a given location, showing the edges explored during shortest-path computation. Useful for visualizing and debugging routing behavior. Note: this endpoint is subject to stricter rate limiting on the public demo server.

- **Human URL:** [https://valhalla.github.io/valhalla/api/expansion/api-reference/](https://valhalla.github.io/valhalla/api/expansion/api-reference/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Expansion
- Graph
- GeoJSON
- Debugging

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/api/expansion/api-reference/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Valhalla Locate API

Provides detailed metadata about graph nodes and edges near a given coordinate. Returns snapped node information, edge attributes, and road network properties for analysis and debugging of routing graph data.

- **Human URL:** [https://valhalla.github.io/valhalla/api/locate/api-reference/](https://valhalla.github.io/valhalla/api/locate/api-reference/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Locate
- Graph
- Metadata
- Debugging

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/api/locate/api-reference/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Valhalla Status API

Returns information about the running Valhalla server instance, including tileset availability and configuration details. Useful for health checks and monitoring the operational status of a Valhalla deployment.

- **Human URL:** [https://valhalla.github.io/valhalla/](https://valhalla.github.io/valhalla/)
- **Base URL:** `https://valhalla1.openstreetmap.de`

#### Tags

- Status
- Health
- Monitoring

#### Properties

- [Documentation](https://valhalla.github.io/valhalla/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [Git Hub](https://github.com/valhalla/valhalla)
- [Documentation](https://valhalla.github.io/valhalla/)
- [OpenAPI](https://valhalla.github.io/valhalla/api/openapi/) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Demo Server](https://valhalla.openstreetmap.de/)
- [License](https://github.com/valhalla/valhalla/blob/master/LICENSE.md)
- [Rate Limits](https://raw.githubusercontent.com/api-evangelist/valhalla/refs/heads/main/rate-limits/openstreetmap-de.yml)
- [Plans](https://raw.githubusercontent.com/api-evangelist/valhalla/refs/heads/main/plans/open-source.yml)
- [Fin Ops](https://raw.githubusercontent.com/api-evangelist/valhalla/refs/heads/main/finops/self-hosted.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
