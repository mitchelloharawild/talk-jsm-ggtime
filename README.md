

<!-- README.md is generated from README.qmd. Please edit that file -->

# ggtime: Visualizing time with a grammar of temporal graphics

<!-- Doesn't have enough stats, be more declarative // on-the-nose.. Improving viz of time series with... -->

<!-- badges: start -->

<!-- badges: end -->

Slides and notes for a presentation about ggtime at JSM 2025 (5th August
2025).

<!-- A recording of this presentation is available on YouTube here: <https://www.youtube.com/watch?v=> -->

<!-- [![](preview.jpg)](https://www.youtube.com/watch?v=) -->

#### Abstract

<!--
&#10;> Linking 'statistical graphics' to modelling and communicating temporal patterns
Effective use of statistical graphics in exploratory time series analysis helps to uncover temporal patterns needed to accurately specify models.
&#10;> Visual idioms -> temporal grammar
While several commonly used plots exist for visualizing time series, little work has been done to formalize them within a unified grammar of temporal graphics.
&#10;> Grammar elements
Decomposing traditional time series graphics such as time plots and seasonal plots into modular grammatical elements provides the flexibility needed to clearly visualize multiple seasonality, cycles, and other complex patterns.
&#10;> Calendrical patterns are central to the temporal grammar
Temporal data visualization requires special handling to highlight patterns shaped by calendar systems, much like the nuances of spatial, graph, and uncertainty visualization.
&#10;> Specific examples from the grammar
The proposed grammar incorporates calendrical concepts to visually align time points at different granularities and timezones, warp time to standardize irregular cyclical durations, and wrap time into hierarchical calendar layouts.
&#10;> Introduce the ggtime package implementation for ggplot2
In this talk, I will introduce the grammar of temporal graphics as implemented in the ggtime R package, and demonstrate how these grammatical elements can be combined to create both familiar and novel visualizations of complex time series patterns.
&#10;-->

Effective use of statistical graphics in exploratory time series
analysis helps to uncover temporal patterns needed to accurately specify
models. While several commonly used plots exist for visualizing time
series, little work has been done to formalize them into a unified
grammar of temporal graphics. Decomposing traditional time series
graphics such as time plots and seasonal plots into modular grammatical
elements provides the flexibility needed to clearly visualize multiple
seasonality, cycles, and other complex patterns.

Temporal data visualization requires special handling to highlight
patterns shaped by calendar systems, much like the nuances of spatial,
graph, and uncertainty visualization. The proposed grammar incorporates
calendrical concepts to visually align time points at different
granularities and timezones, warp time to standardize irregular cyclical
durations, and wrap time into hierarchical calendar layouts. In this
talk, I will introduce the grammar of temporal graphics as implemented
in the ggtime R package, and demonstrate how these grammatical elements
can be combined to create both familiar and novel visualizations of
complex time series patterns.

#### Structure

Slide progression:

- Introduction and background
  - Time plots: the basics of time series visualization
  - Time series patterns: trend, seasonality, cycles, holidays, events,
    …
  - Visualizing seasonality requires more than simply treating time
    continuously
  - Seasonal plots and sub-series plots (time within and across
    ‘seasons’)
  - Outlink to discussion posts by authors about plot helper monoliths
- A grammar of temporal graphics
  - Re-characterizing these plot helpers into modular grammatical
    elements
  - Some discussion on visualization with grammars vs helpers
    (flexible/complex)
  - Design goals and philosophy of ggtime
    - Calendars as the core concept
    - Focus on the temporal dimension (outlink to earlier ggdist talk)
  - ggtime in ggplot2’s layered grammar of graphics
    - Overview of the layered grammar of graphics (data, aes, geom,
      stat, facet, coord)
    - Data: Briefly in calcal/mixtime
    - Aes/Geom: `geom_time_line()`, and other `geom_time_***()`
      geometries
    - Stat: Visually adjust time into civil/absolute, warping cycles,
      and aligning granularities
    - Coord/Facet: Easy calendar layouts
- Using ggtime
  - Re-expressing common time series plots with the grammar
  - Remixing elements to create new time series plots

Presentation narratives:

- Primary: Introducing ggtime
- Secondary: Plot helpers and grammar extensions

### Format

- 20 minutes (+-questions?)
