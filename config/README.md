# Configuration Files

This directory contains the game data configuration files for the Against The Storm Species Needs tool.

## Files

### species.json
Contains data for all playable species including:
- Species name, icon, and image path
- Complex food needs
- Service needs
- Clothing needs

### recipes.json
Contains recipes for all needs (complex food, clothing, and services) including:
- Building name that can produce the item
- Star rating (1-3) indicating efficiency
- Required ingredients
- Worker requirement flag for services

### ingredientRecipes.json
Contains recipes for secondary ingredients needed by main recipes, including:
- Building name that can produce the ingredient
- Star rating (1-3)
- Required base ingredients

## Format

All files use standard JSON format with proper structure for easy maintenance and updates.

## Usage

These files are automatically loaded by the application at startup via the `loadConfigFiles()` function in `index.html`.
