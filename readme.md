# Zoomer's Sliders

![Zoomer's Sliders](zoomers-sliders-s.jpg)

Zoomer's Sliders is an interactive web-based presentation tool built using [OpenSeadragon](https://openseadragon.github.io/). It allows you to load a large image, define multiple zoomable regions, and then navigate through these "slides" in a fullscreen presentation mode.

**Author:** lin.wang@wangscience.com
**Date:** 2024-12-14
**Version:** 1.0.0

## Features

- **Modern Side-by-Side Layout:**  
  A clean, intuitive interface with a collapsible toolbar on the left and the main viewer on the right.

- **Region Selection:**  
  Click and drag to select rectangular regions on the image. These regions will be zoomed into during the presentation mode.
  
- **Monitor-Based Aspect Ratio:**  
  The selected region is always forced to match the aspect ratio of your monitor's screen, ensuring consistent viewing regardless of the browser window size.
  
- **Fullscreen Presentation Mode:**  
  After finalizing your selections, click "Enter Presentation" to enter a fullscreen slideshow mode. You can navigate through the selected regions using:
  - **SPACE** or **→** to move to the next region
  - **←** to move to the previous region
  - **Click** anywhere to also advance to the next region
  - **ESC** to exit fullscreen and return to the overview mode
  
- **Slide Management:**
  - Name your slides for easy identification
  - Reorder slides using up/down controls
  - Remove individual slides as needed
  - Clear all slides with Ctrl+C
  
- **Settings Management:**
  - Save your slide settings as JSON for later use
  - Load previously saved settings to restore your presentation
  - Settings are automatically named based on the source image

- **UI Flexibility:**
  - Toggle the toolbar visibility for a cleaner view
  - Quick access button to restore the UI when hidden
  - Consistent instructions and author info

## Usage

1. **Load Your Image:**  
   Click "Load Image" and select any image file from your computer.
   
2. **Select Regions:**  
   - Click and drag to define rectangular regions. Each region maintains your monitor's aspect ratio.
   - Each region becomes a slide that can be named and reordered.
   - Click "Select Regions" to add more regions at any time.

3. **Manage Slides:**
   - Name your slides using the text inputs
   - Reorder slides using the up/down arrows
   - Remove unwanted slides using the X button
   - Click "Clear All" or press Ctrl+C to start fresh

4. **Finalize Your Selection:**  
   Click "Finalize Regions" when you're done selecting all regions you need.

5. **Save/Load Settings:**
   - Click "Save Settings" to export your slides configuration
   - Use "Load Settings" to restore a previously saved configuration
   - Settings are saved as JSON files named after your image

6. **Enter Presentation Mode:**  
   Click "Enter Presentation" for fullscreen mode. Navigate through slides using arrow keys, space, or click. Press ESC to exit.

## Technical Notes

- Built upon [OpenSeadragon](https://openseadragon.github.io/) for deep zoom capabilities
- Automatic aspect ratio maintenance using screen dimensions
- Responsive design with flexible UI layout
- Settings saved in JSON format for easy sharing and restoration
- Supports both local and CDN-based OpenSeadragon loading
- Tested on modern browsers with fullscreen API support

## License

This project is provided as-is. No specific license has been applied, but feel free to adapt and use it for personal or educational purposes.
