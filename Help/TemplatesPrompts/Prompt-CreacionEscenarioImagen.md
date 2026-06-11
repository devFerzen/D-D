Create a top-down D&D battle map.

STYLE:
- Highly detailed fantasy dungeon.
- Realistic stone architecture.
- Tactical RPG battlemap.
- Overhead camera (90° top-down).
- Designed for virtual tabletop use.
- Clean visibility for tokens and miniatures.

GRID:
- Visible square grid covering the entire map.
- Every square represents 2 meters.
- Grid must be subtle but clearly readable.
- Coordinates must be displayed.

COORDINATES:
- Numbers along the TOP border:
  1, 2, 3, 4, 5, 6, 7, 8...
- Letters along the LEFT border:
  A, B, C, D, E, F, G...
- Coordinates must look like tabletop map rulers.
- Coordinates integrated into the map border.
- No coordinates on the right side.
- No coordinates on the bottom side.

MATRIX:
- Use explicit matrix limits provided by DM.
- Rows range: [FILA_INICIAL]-[FILA_FINAL]
- Columns range: [COLUMNA_INICIAL]-[COLUMNA_FINAL]
- Keep all walkable and relevant tactical zones inside this matrix.
- Do not crop tactical space outside the declared matrix.

SCALE:
- Include a small text label:
  "1 Square = 2 meters"
- Place it in a corner.
- Keep it minimal and unobtrusive.

RESTRICTIONS:
- No character markers.
- No player names.
- No speech bubbles.
- No UI panels.
- No status boxes.
- No arrows.
- No labels on objects.
- No extra text except coordinates and scale note.

OPTIONAL VISIBLE SYMBOL MODE:
- Use visible symbols on the map only if requested by DM.
- If enabled, allowed symbols are for visible elements only (never hidden DM elements).
- Suggested symbols:
  - NPC visible: N
  - Interactive object visible: O
  - Visible hazard: !
  - Cover/obstacle: #
- Optional short legend allowed only when requested by DM.
- If legend is enabled, place a compact legend in a corner.

TACTICAL LAYOUT INPUT (from DM scene file):
- Doors/exits at coordinates: [LISTA_COORD_PUERTAS]
- Main obstacles/cover at coordinates: [LISTA_COORD_COBERTURAS]
- Interactive objects at coordinates: [LISTA_COORD_INTERACTUABLES]
- Hazard zones at coordinates: [LISTA_COORD_PELIGROS]
- Traversable key paths between points: [LISTA_RUTAS_CLAVE]
- Use visible symbol mode: [SI/NO]
- Include short legend: [SI/NO]

PLACEMENT RULES:
- Respect the tactical layout input as map geometry anchors.
- Keep coordinate readability high around key anchors.
- Do not reveal hidden DM-only elements.
- The final image must remain usable for movement counting by coordinates.
- If symbol mode is OFF, do not place symbols or legend.

SCENE:
[DESCRIBIR AQUÍ LA ESCENA]