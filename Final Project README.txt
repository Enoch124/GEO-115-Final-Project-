Final Project 

## Configuration
Before running the script, ensure the following variables are set correctly:
- `Earthquake_stats_csv`: Path to your input CSV file
- `Earthquakestats_Coordinate`: Path for the output feature class

## Input
- CSV file named "Earthquake stats .csv" containing earthquake data with latitude and longitude coordinates.

## Output
- Point feature class named "Earthquakestats_Coordinate" in the specified geodatabase.

## Process
1. The script sets up the ArcGIS environment.
2. It then uses the `CoordinateTableToPoint` tool to convert the CSV data into point features.
3. The resulting point features are stored in the specified geodatabase.

## Notes
- The script is set to not overwrite existing outputs. If you need to overwrite, change `arcpy.env.overwriteOutput = False` to `True`.
- Ensure your CSV file has columns named "Latitude (°)" and "Longitude (°)" for the coordinate conversion.

## Troubleshooting
- If the script fails to run, ensure all paths are correct and the input CSV file exists.
- Check that you have the necessary permissions to write to the output geodatabase.
- Verify that your ArcGIS Pro license is active and includes the necessary extensions.

