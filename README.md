# Spatial Marvels

Seven buildings that shaped 20th-century architecture, shown as Apple-style spatial depth cards. Each card tilts with your pointer, trackpad or device, and the building lifts out of the frame. Under each card is a full visual story written for architecture students.

**Live site:** https://snehabaid1998-byte.github.io/spatial-marvels/

| | Building | City | Year | Architect |
|---|---|---|---|---|
| 1 | Bauhaus Building | Dessau, Germany | 1926 | Walter Gropius |
| 2 | Fallingwater | Mill Run, Pennsylvania | 1939 | Frank Lloyd Wright |
| 3 | Cathedral of Brasília | Brasília, Brazil | 1970 | Oscar Niemeyer |
| 4 | Sydney Opera House | Sydney, Australia | 1973 | Jørn Utzon |
| 5 | Lotus Temple | New Delhi, India | 1986 | Fariborz Sahba |
| 6 | Guggenheim Museum Bilbao | Bilbao, Spain | 1997 | Frank Gehry |
| 7 | Petronas Twin Towers | Kuala Lumpur, Malaysia | 1998 | César Pelli |

## What each building's story covers

1. **Overview:** why it was built, the big idea, and the lesson for your own work.
2. **Circulation:** a simplified plan with the main route animated, a numbered walk-through, the design lesson and a sketch exercise.
3. **Site and climate:** a plan diagram with north, prevailing wind and sun path, plus location, zoning and how the building answers its climate.
4. **Design decisions:** numbered pins on the photo. The same pins on the 3D card open a callout when you tap them.
5. **Style, materials, timeline,** a century-wide chart comparing all seven, and **sources**.

## How to use it

- **Change building:** swipe or drag sideways, use a two-finger trackpad swipe, press the arrow keys, or tap the page dots.
- **Depth:** move the pointer, or tilt a phone or tablet. On a laptop, **Sense lid tilt** uses the webcam to read how the screen is moving. Camera frames stay in the browser and are never uploaded.
- **Link to one building:** add its name after a `#`, for example `#petronas`.

## How it's built

It is a single `index.html` with no build step and no dependencies apart from the Inter font from Google Fonts. Each photo is split into two layers: a background with the building cut out and the sky filled back in (`*-bg.jpg`), and the building cutout (`*-hero.webp`). The year sits between these layers, as on the iPhone Lock Screen, and CSS 3D transforms separate the layers when the card tilts.

To run it locally, serve the folder with any static server:

```bash
python -m http.server 8000
```

## Accuracy

Facts were checked against published sources in October 2026, and each building's story lists them. Wind directions come from 2019–2023 airport weather records (METAR, via the [Iowa Environmental Mesonet](https://mesonet.agron.iastate.edu/)). The circulation plans are simplified study diagrams, not measured drawings. Use published drawings for measured work.

## Photo credits

The photos come from Wikimedia Commons. The cutouts in `photos/` are derivatives and keep each original's license.

| Building | Photographer | License |
|---|---|---|
| Bauhaus | [JensKunstfreund](https://commons.wikimedia.org/wiki/File:Au%C3%9Fenansichten_des_Bauhaus-Geb%C3%A4udes_in_Dessau_08.jpg) | CC BY-SA 4.0 |
| Fallingwater | [lachrimae72](https://commons.wikimedia.org/wiki/File:Fallingwater3.jpg) | CC0 |
| Cathedral of Brasília | [Roberto Castro / MTur](https://commons.wikimedia.org/wiki/File:Roberto_Castro_Catedral_Metropolitana_de_Nossa_Senhora_Aparecida_Brasilia_DF_(39098957600).jpg) | Public domain |
| Sydney Opera House | [Dietmar Rabich](https://commons.wikimedia.org/wiki/File:Sydney_(AU),_Opera_House_--_2019_--_2130.jpg) | CC BY-SA 4.0 |
| Lotus Temple | [A. Savin](https://commons.wikimedia.org/wiki/File:Lotus_Temple_in_New_Delhi_03-2016.jpg) | Free Art License |
| Guggenheim Bilbao | [José Ligero Loarte](https://commons.wikimedia.org/wiki/File:Museo_Guggenheim_--_2021_--_Bilbao,_Euskadi,_Espa%C3%B1a.jpg) | CC BY-SA 4.0 |
| Petronas Towers | [Marcin Konsek](https://commons.wikimedia.org/wiki/File:2016_Kuala_Lumpur,_Petronas_Towers_(26).jpg) | CC BY-SA 4.0 |

Design and code by Sneha Baid.
