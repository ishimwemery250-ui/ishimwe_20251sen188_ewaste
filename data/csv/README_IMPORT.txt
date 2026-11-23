# E-Waste Rwanda CSV starter dataset

Student: Ishimwe Emery
Student ID: 20251SEN188
Course: INSY 8311

## Important data note
All records in these CSV files are SYNTHETIC, fictional sample data created for database development, demonstrations, and testing. They are not official Rwanda government, recycler, or environmental records. Do not present them as real-world observations.

## Files
1. collection_points.csv — collection locations.
2. waste_categories.csv — categories and hazard levels.
3. waste_collections.csv — collected waste records.
4. recycling_facilities.csv — receiving/processing facilities.
5. transport_assignments.csv — movement of collections to facilities.
6. recycling_records.csv — processing and recycling outcomes.

## Suggested Oracle import order
1. collection_points.csv
2. waste_categories.csv
3. recycling_facilities.csv
4. waste_collections.csv
5. transport_assignments.csv
6. recycling_records.csv

## Data relationships
- waste_collections.collection_point_id -> collection_points.collection_point_id
- waste_collections.waste_category_id -> waste_categories.waste_category_id
- transport_assignments.collection_id -> waste_collections.collection_id
- transport_assignments.facility_id -> recycling_facilities.facility_id
- recycling_records.transport_id -> transport_assignments.transport_id

## Import notes
- Dates use YYYY-MM-DD.
- Quantities are in kilograms (kg).
- Blank delivery_date means the transport has not yet been delivered.
- Use VARCHAR2 for descriptive/status fields, NUMBER for IDs and quantities, and DATE for date fields.
- Create and test the table definitions and constraints before importing.
- Consider loading CSVs into staging tables first, then validating and inserting into final tables.

## Suggested next step
Create the Oracle table definitions to match these column names and relationships, then import the CSV files in the order above.
