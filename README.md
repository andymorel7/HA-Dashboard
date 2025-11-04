# Home Assistant - Minimalistic Dashboard

![Dashboard Preview](https://github.com/user-attachments/assets/8096c365-b4f2-4615-911c-e50ea7e82a94)

A clean, modern, and minimalistic dashboard design for Home Assistant that provides an elegant interface for your smart home.

## Prerequisites

Before installing this dashboard, ensure you have:

- Home Assistant installed and running
- HACS (Home Assistant Community Store) installed
- Basic knowledge of Home Assistant's YAML configuration

## Required HACS Add-ons

You'll need to install the following add-ons from HACS before using this dashboard configuration:

1. **[Card Mod](http://homeassistant.local:8123/hacs/repository/680112919)**
2. **[Layout Card](http://homeassistant.local:8123/hacs/repository/190927524)**
3. **[Bubble Card](http://homeassistant.local:8123/hacs/repository/444350375)**
4. **[Mushroom Cards](http://homeassistant.local:8123/hacs/repository/146194325)**
5. **[Mini Graph Card](http://homeassistant.local:8123/hacs/repository/793248285)**

### Installing HACS Add-ons

1. Open Home Assistant
2. Navigate to **HACS** in the sidebar
3. Click on **Frontend**
4. Search for each add-on by name or use the links above
5. Click **Download** for each add-on
6. Restart Home Assistant after installing all add-ons

## Installation

### Step 1: Create a New Dashboard

![Step 1](https://github.com/user-attachments/assets/dfe1dd6d-64b3-4c0d-a2bd-7eb85386941f)

1. In Home Assistant, click on **Settings** (gear icon in the sidebar)
2. Navigate to **Dashboards**
3. Click the **+ ADD DASHBOARD** button in the bottom right
4. Choose **New dashboard from scratch**
5. Give your dashboard a name (e.g., "Minimalistic Dashboard")
6. Set the icon and other preferences as desired
7. Click **CREATE**

### Step 2: Enter Edit Mode

![Step 2 - Menu](https://github.com/user-attachments/assets/cbb8503d-db0c-46ef-8cee-41c86d1e0cd1)
![Step 2 - Edit](https://github.com/user-attachments/assets/cae915be-b2fa-4304-97e8-d6b41ad7b721)

1. Navigate to your newly created dashboard
2. Click the **three-dot menu** (⋮) in the top right corner
3. Select **Edit Dashboard**

### Step 3: Access Raw Configuration Editor

![Step 3](https://github.com/user-attachments/assets/40231197-c764-4a5a-8a9a-94367c5ccf72)

1. While in edit mode, click the **three-dot menu** (⋮) again
2. Select **Raw configuration editor**
3. This will open a YAML editor

### Step 4: Paste Configuration

![Step 4](https://github.com/user-attachments/assets/add01161-b8ce-4799-9a44-a3cc60b24f0d)

1. Delete any existing YAML code in the editor
2. Copy the entire contents of the `dashboard.yaml` file from this repository
3. Paste it into the Raw configuration editor
4. Click **SAVE** in the top right corner
5. Exit edit mode

## Customization

After installation, you'll need to customize the dashboard to match your Home Assistant entities:

### Updating Entity IDs

The dashboard uses placeholder entity IDs. You'll need to replace them with your actual entities:

1. Enter **Edit Dashboard** mode
2. Open the **Raw configuration editor**
3. Search for entity IDs (e.g., `light.living_room`, `sensor.temperature`)
4. Replace them with your actual entity IDs
5. Save your changes

### Common Entity Types to Update

- Lights (`light.*`)
- Switches (`switch.*`)
- Sensors (`sensor.*`)
- Climate controls (`climate.*`)
- Media players (`media_player.*`)
- Covers/Blinds (`cover.*`)

### Customizing Colors and Styles

This dashboard uses Card Mod for styling. You can customize colors, spacing, and other visual elements by modifying the `card_mod` sections in the YAML configuration.

## Troubleshooting

### Cards Not Displaying

- Ensure all required HACS add-ons are installed
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Restart Home Assistant

### Entity Not Found Errors

- Check that your entity IDs are correct
- Verify entities exist in **Developer Tools** > **States**

### Styling Not Applied

- Ensure Card Mod is properly installed
- Check browser console for errors (F12)

## Support

If you encounter issues:

1. Check that all prerequisites are met
2. Verify HACS add-ons are up to date
3. Review the Home Assistant logs for errors
4. Open an issue in this repository with details about your problem

## Contributing

Contributions are welcome! Feel free to:

- Submit bug reports
- Suggest new features
- Create pull requests with improvements

## License

This project is provided as-is for use with Home Assistant. Feel free to modify and share.

## Acknowledgments

- Home Assistant community
- HACS developers
- All the custom card developers whose work makes this dashboard possible

---

**Note:** Remember to replace all placeholder entity IDs with your actual Home Assistant entities after installation.
