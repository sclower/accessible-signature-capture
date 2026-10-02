# Accessible Signature Capture

Accessible Signature Capture is a small browser-based tool for capturing a handwritten signature, with particular attention to users who cannot visually locate or verify a conventional signature box.

The application is entirely client-side. **Nothing drawn in the signature area is uploaded or transmitted anywhere.**

## Features

- Explore the signature area before drawing.
- Screen-reader announcements indicate when the pointer is on or outside the signature area.
- Press **Space** to turn capture on or off.
- On a laptop touchpad, draw simply by moving your finger while capture is on; no click-and-hold is required.
- **Escape** immediately turns capture off.
- Reports whether a signature was actually detected.
- Saves with tightly cropped whitespace.
- Exports as PNG, JPG, or GIF.
- PNG and GIF preserve transparency; JPG uses a white background.
- **Alt+C** clears the signature.
- **Alt+S** provides a quick PNG save.
- No server, account, dependencies, analytics, or build process.

## Using the Tool

1. Open the page in a modern browser such as Chrome or Edge.
2. Move around until your screen reader announces **“On signature area.”**
3. Press **Space** to turn capture on.
4. On a laptop touchpad, move your finger normally to write your signature. You do not need to press or click the touchpad.
5. Press **Space** again to stop capture.
6. Confirm that the tool announces **“Signature detected.”**
7. Choose **Save PNG**, **Save JPG**, or **Save GIF**.

For a touchscreen or stylus, turn capture on and draw directly in the signature area.

## Keyboard Commands

- **Space:** Toggle capture on/off when focus is not on another interactive control.
- **Escape:** Stop capture.
- **Alt+C:** Clear the signature.
- **Alt+S:** Save as PNG.

## Privacy

Signature data remains in the browser. This project contains no analytics, network requests, server-side processing, or signature storage. Saving creates a local image download.

As with any downloaded signature image, the resulting file itself should be treated as sensitive and stored appropriately.

## Running Locally

There is nothing to install. Download `index.html` and open it in a web browser.

## Publishing with GitHub Pages

1. Create a GitHub repository, for example `accessible-signature-capture`.
2. Put `index.html` and `README.md` in the repository root.
3. Open the repository's **Settings**.
4. Select **Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/(root)`, then save.

The resulting project site will normally be available at:

`https://YOUR-USERNAME.github.io/accessible-signature-capture/`

## Technical Notes

The project uses standard HTML, CSS, JavaScript, Canvas, Pointer Events, and ARIA live-region feedback. It has no external runtime dependencies.

The drawing canvas is automatically cropped to the detected ink before export so the resulting signature file does not contain excessive whitespace.

## Accessibility Feedback

Screen-reader, browser, touchscreen, touchpad, and stylus combinations can behave differently. Accessibility bug reports and improvements are welcome.
