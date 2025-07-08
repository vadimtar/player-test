# FAPlayer Test Page

A static test page for the FAPlayer HTML5 video/audio player that can be deployed via GitHub Pages.

## Features

- **Dynamic Configuration Form**: Based on the `PlayerConfig` TypeScript interface
- **Real-time Player Preview**: See changes immediately when you update settings
- **Comprehensive Settings**: All player configuration options available
- **No Build Tools Required**: Pure HTML, CSS, and JavaScript
- **GitHub Pages Ready**: Can be deployed directly to GitHub Pages

## File Structure

```
/docs
├── index.html            # Main test page with form and player
├── /dist
│   ├── player.js         # Compiled player JavaScript
│   └── player.css        # Compiled player styles
└── README.md             # This file
```

## Usage

1. **Open the Test Page**: Simply open `index.html` in your web browser
2. **Configure the Player**: Use the form on the left to adjust all player settings
3. **Initialize Player**: Click "Initialize Player" to see your configuration in action
4. **Test Features**: The player includes sample video content for testing

## Configuration Options

### Basic Settings
- **Holder Element ID**: The container element for the player
- **Content Mode**: Enable/disable content playback
- **Width/Height**: Player dimensions
- **Player Type**: Video or Audio player
- **Start Volume**: Initial volume level (0-1)
- **Autoplay**: Auto-start playback
- **Viewability Threshold**: Percentage of player that must be visible
- **Show Unmute Button**: Display unmute button for autoplay
- **Show Title**: Display video title overlay

### Content Player Settings
- **Show Volume Slider**: Display volume control
- **Show Duration**: Display time information
- **Show Countdown**: Display countdown timer

### Ads Player Settings
- **Show Volume Slider**: Display volume control for ads
- **Show Duration**: Display time information for ads
- **Show Countdown**: Display countdown timer for ads

### Sticky Settings
- **Sticky Mode**: Disabled, Content Only, Ad Only, or Both
- **Sticky Position**: Bottom Left, Bottom Right, Top Left, or Top Right
- **Margin Bottom**: Distance from bottom edge

### Ads Settings
- **Tag URL**: VAST tag URL for ad serving
- **Preroll**: Enable preroll ads
- **Postroll**: Enable postroll ads
- **Waterfall Cycles**: Number of ad waterfall cycles
- **Midroll Cue Points**: Array of cue points for midroll ads
- **Extra Trackers**: Additional tracking URLs

## Deployment

### Local Testing
Simply open `index.html` in any modern web browser.

### GitHub Pages
1. Push this repository to GitHub
2. Go to repository Settings > Pages
3. Select source branch (usually `main` or `master`)
4. Set folder to `/docs`
5. Your test page will be available at `https://username.github.io/repository-name/`

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Notes

- This test page uses a mock implementation of FAPlayer for demonstration
- The actual player implementation should replace `dist/player.js`
- Sample video content is loaded from Google's sample video CDN
- All configuration options are validated before player initialization

## Troubleshooting

- **Player not loading**: Check that `dist/player.js` and `dist/player.css` exist
- **Form validation errors**: Ensure all required fields are filled
- **Video not playing**: Check browser autoplay policies and mute settings
- **Styling issues**: Ensure CSS file is properly loaded

## Development

To modify the test page:
1. Edit `index.html` for form structure and styling
2. Update `dist/player.css` for player styles
3. Modify `dist/player.js` for player behavior
4. Test locally before deploying 