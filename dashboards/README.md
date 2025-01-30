# FiatChamp Dashboards

This directory contains pre-made dashboards for the FiatChamp Home Assistant addon. These dashboards are designed to work with various vehicle models supported by the addon.

## Available Dashboards

- `jeep_dashboard.yaml` - Comprehensive dashboard for Jeep vehicles

## Installation

1. Prerequisites:
   - Home Assistant with FiatChamp addon installed and configured
   - HACS (Home Assistant Community Store) installed
   - [auto-entities](https://github.com/thomasloven/lovelace-auto-entities) custom card installed from HACS

2. Dashboard Installation:
   - Go to Home Assistant Settings → Dashboards
   - Click the "+" button in the bottom right corner to add a new dashboard
   - Give your dashboard a name (e.g., "Jeep Grand Cherokee L")
   - Once created, click the three dots menu on your new dashboard and select "Edit Dashboard"
   - Click the three dots menu again and select "Raw configuration editor"
   - Delete any existing content and paste the entire contents of `jeep_dashboard.yaml`
   - Click "Save" to apply the changes

## Dashboard Features

### Main View
- Interactive map showing vehicle location
- Current vehicle status
  - Location
  - Odometer
  - Fuel levels and range
  - Last update time
- Quick action buttons
  - Update location
  - Blink lights
  - Door lock/unlock
  - Trunk control
  - Vehicle status refresh

### Details View
- Tire pressure monitoring
  - Automatic display of all tire pressures
  - Pressure warnings and status
- Trip information
  - Trip A and Trip B statistics
  - Distance traveled
  - Fuel economy
- Vehicle health
  - Oil level
  - Battery voltage
  - Battery status

### Service View
- Service tracking
  - Days until next service
  - Distance to service
- Addon updates

## Customization

You can customize the dashboard by editing the YAML file. Common customizations include:

- Changing the layout of cards
- Adding or removing entities
- Modifying card titles and icons
- Adjusting the map zoom level

To customize:
1. Open the dashboard YAML file in a text editor
2. Make your desired changes
3. Save the file
4. Refresh your Home Assistant page

## Troubleshooting

1. **Unknown Entities**
   - Some entities might show as "unknown" until the vehicle sends its first update
   - Use the "Refresh Vehicle Status" button to trigger an update

2. **Missing Cards**
   - Ensure all required custom cards are installed through HACS
   - Check that the entity IDs match your vehicle's entities

3. **Map Not Showing**
   - Verify that location tracking is enabled in FiatChamp
   - Check that your Home Assistant instance has a valid location configured

## Support

If you encounter issues or need help customizing your dashboard:
1. Check the [FiatChamp GitHub repository](https://github.com/wubbl0rz/FiatChamp) for known issues
2. Join the discussion in the Home Assistant community forums
3. Open an issue on GitHub if you find a bug

## Contributing

Feel free to contribute your own dashboard designs or improvements:
1. Fork the repository
2. Create your dashboard or make improvements
3. Submit a pull request with your changes

## License

These dashboards are released under the same license as the FiatChamp project.