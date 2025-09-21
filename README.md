# EKS EUP Wardrobe

This script is a lightweight, fully configurable EUP wardrobe menu with a clean custom UI.  
It allows you to define organisations, categories, and outfits in a simple `config.lua`, and players can easily select outfits in-game.

## Features
- Custom UI with categories & subcategories 
- Fully configurable outfits in `config.lua`
- Category descriptions and outfit thumbnails
- ESC or Close button to exit menu
- `/eup` command to open the wardrobe
- Automatically applies outfits with both components and props

## Installation

1. Drag and drop the folder into your `resources/` directory  

2. Add the following to your `server.cfg`:
ensure EKS_EUP

3. Configure your outfits inside `config.lua`. Example:

Config.Catalog = {
  {
    org = "New Hartshire Constabulary",
    children = {
      {
        name = "Frontline Policing",
        description = "Standard frontline patrol uniforms",
        outfits = {
          { label = "Patrol Uniform", components = { torso = {3,0}, pants = {24,0}, shoes = {10,0} }, props = { hat = {1,0} } },
          { label = "High-Vis Jacket", components = { torso = {11,2}, pants = {24,0}, shoes = {10,0} } }
        }
      }
    }
  }
}

## Usage

Type /eup in chat to open the wardrobe UI.

Select your organisation, category, and outfit.

Press ESC or the Close button to exit the menu.

Support
For help or customization, open a ticket through EKS.

discord.gg/busQ9w6dqa
