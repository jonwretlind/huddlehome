# Assets Folder Structure

This folder contains all the static assets for the HuddleHome landing page.

## 📁 Folder Structure

```
assets/
├── css/
│   └── styles.css          # Main stylesheet
├── js/
│   └── script.js           # Main JavaScript file
├── images/
│   ├── family-background.svg           # SVG family illustration
│   └── family-photo-placeholder.svg    # Placeholder for real family photo
└── README.md               # This file
```

## 🖼️ Images

### Current Images:
- **family_hero_background_optimized.jpg**: Family photo (part of hero background slider)
- **family2_hero_background_left_aligned_optimized.jpg**: Family photo (part of hero background slider)
- **family3_hero_autumn_optimized.jpg**: Autumn family photo (part of hero background slider)
- **family-background.svg**: SVG illustration of family silhouettes (backup)

### Recommended Family Photo:
To replace the placeholder with a real family photo:

1. **File Format**: JPG or PNG
2. **Dimensions**: 800x600px or larger (will be scaled)
3. **Content**: Family playing together, having fun
4. **Style**: Bright, warm, family-oriented
5. **File Name**: `family-photo.jpg` or `family-photo.png`

### How to Replace:
1. Add your family photo to `assets/images/`
2. Update the CSS file `assets/css/styles.css`:
   ```css
   background-image: url('../images/your-family-photo.jpg');
   ```

## 🎨 Design Guidelines

- **Colors**: Use the HuddleHome brand colors when possible
- **Style**: Keep images bright, family-friendly, and modern
- **Optimization**: Compress images for web use
- **Accessibility**: Ensure good contrast and readability

## 🎬 Background Slider

The hero section features an animated background slider that cycles through three family photos:

1. **family_hero_background_optimized.jpg** - Main family photo
2. **family2_hero_background_left_aligned_optimized.jpg** - Left-aligned family photo  
3. **family3_hero_autumn_optimized.jpg** - Autumn-themed family photo

### Slider Features:
- **Duration**: 18 seconds per cycle (12 seconds on mobile)
- **Transition**: Smooth fade between images
- **Performance**: Optimized for mobile devices
- **Overlay**: Subtle gradient overlay for text readability

## 📝 Notes

- All file paths in CSS are relative to the CSS file location
- JavaScript paths in HTML are relative to the root directory
- Images should be optimized for web performance 