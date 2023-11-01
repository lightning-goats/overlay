# Lightning Goats Livestream OBS Overlay

## Description

This is an HTML overlay designed to be used with OBS Studio for the Lightning Goats Livestream. The overlay has several features, including:

- A QR Code display for donations.
- A progress bar indicating the progress towards a specific donation goal.
- Displaying comments in a scrolling fashion.
- Different types of notifications like "Feeder Triggered".

## Technologies

- HTML5
- CSS3
- JavaScript
- WebSocket API for real-time updates

## Setup

1. Clone the repository or download the HTML file.
2. In OBS Studio, add a new "Browser" source and point it to the local HTML file.
3. Customize the overlay dimensions to match your OBS Studio canvas (1280x720 is the default).

## File Structure

- **index.html**: Main HTML file containing the structure of the overlay.
- **styles.css** (embedded in HTML): Contains the styling for the overlay.
- **script.js** (embedded in HTML): Contains the JavaScript logic for real-time updates and interactions.

### Main Components

#### QR Code and Sats Left

- `#qr-code`: Element displaying the QR code for donations.
- `#sats_left`: Element displaying the number of satoshis left to reach the goal.

#### Progress Bar

- `#progress-container`: Container for the progress bar.
- `#progress-fill`: Filling part of the progress bar.
- `#progress-text`: Text overlay on the progress bar.

#### Comments

- `.scrolling-comment`: Class for the scrolling comments.
- `#comment-container`: Container for the comments.

#### Notifications

- `#goal-achieved-layer`: Layer shown when the goal is achieved.
- `#feeder-triggered`: Notification for "Feeder Triggered".

## Customization

You can modify the `goalDollars` and `WS_URL` variables in the JavaScript code to set the donation goal and WebSocket URL.

## Contributing

Feel free to fork the project and submit a pull request for any features or fixes.

## License

This project is open source under the MIT license.
