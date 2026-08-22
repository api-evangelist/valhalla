# Valhalla (valhalla)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
