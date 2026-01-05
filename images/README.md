# Game Assets Directory

This directory contains icons and images from the game "Against the Storm" by Eremite Games.

## Directory Structure

- **species/**: Icons for each playable species (Humans, Beavers, Lizards, Harpies, Foxes, Frogs, Bats)
- **food/**: Icons for complex food items (Biscuits, Jerky, Pickled Goods, Pie, Skewers, Porridge, Paste)
- **clothing/**: Icons for clothing items (Coats, Boots)
- **services/**: Icons for services (Leisure, Religion, Education, Cleanliness, Brawling, Luxury)
- **buildings/**: Icons for buildings that produce goods and services
- **ingredients/**: Icons for raw materials and intermediate ingredients

## Image Format

All images should be in PNG format with transparent backgrounds where appropriate.

Recommended image sizes:
- Species icons: 64x64px or 128x128px
- Food/Clothing/Service icons: 48x48px or 64x64px
- Building icons: 64x64px or 128x128px
- Ingredient icons: 48x48px or 64x64px

## Naming Convention

Files should be named using lowercase with hyphens:
- `humans.png`, `beavers.png`, `lizards.png`, etc.
- `biscuits.png`, `jerky.png`, `pickled-goods.png`, etc.
- `coats.png`, `boots.png`
- `leisure.png`, `religion.png`, etc.

## How to Add Images

You have two options for adding game icons to this tool:

### Option 1: Hotlink to Official Wiki Assets (Recommended)

You can directly link to images hosted on the official wiki. This avoids the need to download and store images locally.

**To find wiki image URLs:**

1. Visit the [Against the Storm Official Wiki](https://wiki.hoodedhorse.com/Against_the_Storm/Against_the_Storm_Official_Wiki)
2. Navigate to a species, item, or building page (e.g., [Humans](https://wiki.hoodedhorse.com/Against_the_Storm/Humans))
3. Right-click on an image/icon and select "Open image in new tab"
4. Copy the full URL from your browser's address bar
   - URLs typically follow the format: `https://wiki.hoodedhorse.com/images/[hash]/[hash]/[filename]`
   - Example: `https://wiki.hoodedhorse.com/images/3/3d/Forum.png`

**To use hotlinked images:**

Edit `index.html` and update the `image` property in the `speciesData` object to use the full wiki URL instead of a local path:

```javascript
humans: {
    name: 'Humans',
    icon: '👤',
    image: 'https://wiki.hoodedhorse.com/images/x/xx/Human_icon.png',  // Replace with actual URL
    // ...
}
```

The system automatically validates that hotlinked URLs are from the official wiki (`wiki.hoodedhorse.com`) for security.

### Option 2: Download and Store Locally

Alternatively, you can download icons from the wiki and store them in the `images/` directory.

**Steps:**

1. Visit the [Against the Storm Official Wiki](https://wiki.hoodedhorse.com/Against_the_Storm/Against_the_Storm_Official_Wiki)
2. Navigate to relevant pages for species, items, or buildings
3. Right-click on icons and select "Save image as..."
4. Save files to the appropriate subdirectory:
   - `images/species/` for species icons (humans.png, beavers.png, etc.)
   - `images/food/` for food items (biscuits.png, jerky.png, etc.)
   - `images/clothing/` for clothing (coats.png, boots.png)
   - `images/services/` for services (leisure.png, religion.png, etc.)
   - `images/buildings/` for building icons
   - `images/ingredients/` for ingredient icons
5. Ensure filenames match the naming convention (lowercase with hyphens)
6. The web application will automatically use these images instead of emoji fallbacks

### Image Format Guidelines

- **Format:** PNG with transparent backgrounds (when appropriate)
- **Recommended sizes:**
  - Species icons: 64x64px or 128x128px
  - Food/Clothing/Service icons: 48x48px or 64x64px
  - Building icons: 64x64px or 128x128px
  - Ingredient icons: 48x48px or 64x64px

### Credits

All game assets are property of **Eremite Games** and **Hooded Horse** (publisher) and are used for fan-made tools to enhance the gaming experience. 

**Against the Storm** is developed by Eremite Games and published by Hooded Horse.
- Official Wiki: https://wiki.hoodedhorse.com/Against_the_Storm/Against_the_Storm_Official_Wiki
- Developer Website: https://eremitegames.com/
- Publisher Website: https://hoodedhorse.com/
- Steam: https://store.steampowered.com/app/1336490/Against_the_Storm/
