# Zoomer's Sliders

![Zoomer's Sliders](zoomers-sliders.webp)

Zoomer's Sliders is an interactive web-based presentation tool built using [OpenSeadragon](https://openseadragon.github.io/). It allows you to load a large image, define multiple zoomable regions, and then navigate through these "slides" in a fullscreen presentation mode.

**Author:** lin.wang@wangscience.com
**Date:** 2024-12-14
**Version:** 0.1.0

## Features

- **Region Selection:**  
  Click and drag to select rectangular regions on the image. These regions will be zoomed into during the presentation mode.
  
- **Monitor-Based Aspect Ratio:**  
  The selected region is always forced to match the aspect ratio of your monitor's screen, ensuring consistent viewing regardless of the browser window size.
  
- **Fullscreen Presentation Mode:**  
  After finalizing your selections, press 'P' to enter a fullscreen slideshow mode. You can navigate through the selected regions using:
  - **SPACE** or **→** to move to the next region
  - **←** to move to the previous region
  - **Click** anywhere to also advance to the next region
  - **ESC** to exit fullscreen and return to the overview mode
  
- **Reset Anytime:**  
  Press **Ctrl+C** to clear all selected regions and start fresh at any time.
  
- **Consistent Instructions and Author Info:**  
  The instructions panel is always visible and updates depending on the mode (editing or presentation). Author info is consistently displayed.

## Usage

1. **Load Your Image:**  
   Ensure `pp.png` is placed in the same directory as the `index.html` file (or adjust the code to point to your image).
   
2. **Open in a Browser:**  
   Simply open `index.html` in a modern browser. The tool will load the image via OpenSeadragon.

3. **Select Regions:**  
   - Click and drag to define a rectangular region. A single click without dragging will not create a region.
   - Each region will be recorded as soon as you release the mouse button if it's large enough.

4. **Finalize Your Selection:**  
   Press **E** when you're done selecting all regions you need. The instructions will update accordingly.

5. **Enter Presentation Mode:**  
   Press **P** to enter fullscreen slideshow mode. Use SPACE/→, ←, or click to navigate through your defined regions. Press ESC to exit fullscreen and return to the overview.

6. **Reset if Needed:**  
   Press **Ctrl+C** at any time to clear all selections and return to the initial state.

## Technical Notes

- Built upon [OpenSeadragon](https://openseadragon.github.io/) for deep zoom capabilities and custom interaction tracking.
- Utilizes `window.screen.width` and `window.screen.height` to determine the aspect ratio, ensuring stability across browser window resizing.
- The code is self-contained in a single HTML file with embedded JavaScript and CSS.
- Tested primarily on modern browsers. Fullscreen functionality and ESC behavior may vary slightly by operating system (notably macOS).

## License

This project is provided as-is. No specific license has been applied, but feel free to adapt and use it for personal or educational purposes.
