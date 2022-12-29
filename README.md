# Proof of Concept: FE UI to mutate SVG and then render as image 

## Requirements

- Given any SVG, a user can manipulate certain properties via UI
    - Stroke and Fill for most cases
    - Requires all 'canned' assets be prepped
- FE should take mutated SVG and output as image with alpha layer intact
    - Use HTMLCanvas to generate snapshot of SVG
    - For this PoC, output as PNG
    - Right-click to save as image (in lieu of implementing a Post to some API)

## Running

All files are standalone.  No webserver required.

Open `index.html` in your browser and manipulate the colors by updating the text boxes.  UI to mutate SVG on left and rendered PNG on right.  Right-click to save the PNG in local folder as `testsave.png`

Open `testsave.html` to view the PNG on a yellow background, to demonstrate the alpha layer is intact, as evidenced by the slight shadow gradient.