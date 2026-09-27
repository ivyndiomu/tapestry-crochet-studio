# Testing strategy

## Why testing matters here

Some defects can create physical rework. A row-direction error, garment-shaping error or yarn-count error can affect an item that takes hours or days to make.

Testing is therefore part of product quality, not only engineering hygiene.

## Regression areas

### Gauge and conversion

- non-square gauge correction
- crop-aware row calculation
- crop boundary clamping
- conversion settings preserving crop state

### Grid editing

- connected flood fill
- line and rectangle drawing
- selection copy, move and replace
- pattern flips
- masked editing on garment cells

### Crochet intelligence

- bottom-up row numbering
- alternating working direction
- colour-change analysis
- short/small region warnings
- yarn calibration behaviour

### Garment and construction

- physical panel dimensions to stitch/row counts
- artwork centring and fit
- oversized artwork movement
- neckline and armhole construction
- sleeve working direction and decreases
- physical stitch counts excluding cut-out cells

### Yarn and production

- colour-distance matching
- stock-aware matching and substitution
- skein planning
- production progress
- timer/session accumulation

### Exports and business workflow

- paper dimensions and tiled charts
- bottom-up chart labels
- written instructions
- quote totals, deposit logic and currency behaviour
- order status progression

### Project model

- older project migration
- multi-panel switching
- design duplicate/move behaviour
- panel-specific palette state
- freestyle-origin preservation

## Release gate

A product increment is not complete until:

- the problem and user job are documented
- acceptance criteria and failure states are defined
- migration impact is understood
- relevant regression tests pass
- affected exports are visually checked
- user-visible changes are recorded
- a real crochet project exercises production logic where applicable
