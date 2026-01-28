# Custom Icons

## Mana Icon

To use a custom mana icon instead of the default Lucide Zap icon:

1. **Add your PNG file**: Place your transparent background PNG at `/public/icons/mana-icon.png`
   - Recommended size: 64x64px or larger (will scale automatically)
   - Format: PNG with transparent background
   - Style: Should match the game's art style

2. **Enable custom icon**: Open `/src/components/Common/ManaIcon.jsx` and change:
   ```javascript
   const USE_CUSTOM_ICON = false;  // Change to true
   ```

3. **Restart the development server** to see the changes

## File Structure

```
/public/icons/
├── README.md          # This file
└── mana-icon.png      # Your custom mana icon (add this)
```

## Notes

- The icon will automatically inherit colors from the component's className
- If you need to adjust the icon path, edit the `CUSTOM_ICON_PATH` constant in `ManaIcon.jsx`
- The icon is used in the main header resource display
