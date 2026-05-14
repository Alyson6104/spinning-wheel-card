# 🎡 spinning-wheel-card - Add interactive spin wheels to Home Assistant

[![](https://img.shields.io/badge/Download-Spinning_Wheel_Card-blue.svg)](https://github.com/Alyson6104/spinning-wheel-card)

This software allows you to create interactive, spinning wheels inside your Home Assistant dashboard. You can use these wheels to make random choices or gamify your home automation tasks. It supports drag-and-flick motion, plays audio when the wheel hits pins, and includes physics-based movement.

## ⚙️ System Requirements

You need a working Home Assistant instance to use this card. Ensure you have the HACS (Home Assistant Community Store) integration installed before you begin. This card works on all modern web browsers including Chrome, Firefox, Edge, and Safari. You do not need to install extra software on your computer.

## 📥 Getting the Files

Visit the [official repository page](https://github.com/Alyson6104/spinning-wheel-card) to access the latest version of the card. 

1. Open your web browser.
2. Navigate to the link above.
3. Locate the section labeled Releases on the right side of the page.
4. Click the version number or the link titled "Releases."
5. Download the file named `spinning-wheel-card.js` to your computer.

Keep this file in a location you can easily find, such as your Downloads folder.

## 🛠️ Installation through HACS

The easiest way to add this card to Home Assistant is through HACS. Follow these steps to complete the setup.

1. Open your Home Assistant dashboard.
2. Click on the HACS menu item in the sidebar.
3. Select Frontend.
4. Look for the three dots in the top right corner.
5. Choose "Custom repositories."
6. Paste the URL of the repository (https://github.com/Alyson6104/spinning-wheel-card) into the box.
7. Select "Lovelace" as the category.
8. Click Add.
9. Find "Spinning Wheel Card" in your list and click Download.
10. Refresh your browser page to ensure Home Assistant loads the new file.

## 📝 Configuring the Card

Once the card is installed, you must add it to your dashboard. 

1. Navigate to your Home Assistant dashboard.
2. Click the three dots in the top right corner.
3. Select "Edit Dashboard."
4. Click the "Add Card" button.
5. Search for "Spinning Wheel Card" in the list of available cards.
6. Select the card. 

The configuration screen opens. This interface lets you modify the behavior and appearance of the wheel. You can define labels for each segment, set the weight or size of slices, and choose custom colors. 

### Customizing Labels and Colors
In the configuration editor, you will see a text block. This area allows you to define the segments of your wheel. Enter your items as a list. You can assign a specific color to each segment to make the wheel look unique. If you leave the color option blank, the system chooses colors for you.

### Adding Labels and Weights
You can adjust the probability of where the wheel lands by changing the weight values. Higher numbers increase the chance that the wheel lands on a specific segment. You can also translate your labels into English or German, as both languages are built into the system.

### Sound Effects
The card includes a peg-click sound feature. This sound plays whenever a pin on the wheel passes the indicator. You can toggle this sound on or off in the configuration menu. 

## 🖱️ Using the Wheel

After you save the configuration, the wheel appears on your dashboard. You can interact with it using your mouse or touch screen.

* Click and hold the wheel to spin it.
* Drag your cursor across the wheel in a flicking motion to create momentum.
* Watch the physics engine slow the wheel down until it reaches a complete stop.
* The system detects the final segment and executes the command associated with that choice.

## 🔧 Troubleshooting

If the card does not appear on your dashboard after installation, try these steps:

* Clear your browser cache. Sometimes the browser displays an old version of your dashboard.
* Ensure you click "Refresh" in the HACS Frontend menu.
* Check that you added the card to the specific dashboard view you are currently viewing.
* Verify your YAML configuration if you are using the code editor. Look for syntax errors like missing commas or quotation marks.

If you continue to experience issues, verify that your Home Assistant core is up to date. This card requires a reasonably recent version of Home Assistant to handle the Shadow DOM and Lit framework requirements.

## 💡 Tips for Best Results

* Use high-contrast colors for your labels so they remain readable as the wheel spins.
* Keep your labels short to ensure they fit inside the wheel segments.
* Use the weight feature to influence common choices, such as setting a higher weight for the "Do Nothing" option.
* Add multiple wheels to different tabs to organize your choices by category.

This card operates locally on your Home Assistant server, which ensures your data stays private and your automations remain fast. It uses the Lit library to maintain high performance even when you have multiple wheels running at once.