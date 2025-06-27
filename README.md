This project is for a simple GSheets tool to sum water takes from any point on the BOP water network.
Key bits are:
1) 2 scripts that the spreadsheets uses to upload new consent data into ther api - prefixed sheet.
2) The spreadsheet itself. This contains the full Rec 2.4 network plus a geospatial join of Rec and BOP consent.
The joined GIS data is static due to BOPRC not sharing sufficient data to fully automate the whole project.
Index.html which houses a small leaflet js.script which allows a user to select a location on a map and pushes
that location ID to the spreadsheet triggerring a recalculation of the upstream network .. which in turn collates
all consents on or above that point. There may be duplicate consents so a second table contains aggregate calculations.
