# E-Waste Rwanda

**Project title:** Rwanda Electronic Waste Collection, Recycling and Environmental Compliance Tracking System  
**Student:** Ishimwe Emery  
**Student ID:** 20251SEN188  
**Course:** INSY 8311 – Database Development with PL/SQL  
**Group:** Wednesday Group C  
**GitHub:** https://github.com/ishimwemery250-ui/ishimwe_20251sen188_ewaste

## Project overview
This academic project proposes an Oracle Database and PL/SQL application for recording electronic-waste collections, tracking transportation to processing facilities, recording recycling outcomes, and producing operational reports.

## Important academic and data notes
- The CSV records in `data/csv/` are synthetic sample data for development and testing. They are not official Rwanda records or statistics.
- Verify all proposed requirements and any external sources before relying on them in the final submission.
- The assignment restricts AI assistance for the Phase I business-process analysis/diagram. That deliverable is intentionally not generated or included here; complete it independently according to the instructor's instructions.
- Project registration does not equal instructor approval. Confirm topic uniqueness and approval with the instructor.

## Repository structure
- `docs/proposal/` — project proposal
- `docs/presentation/` — project presentation
- `docs/research/` — research log template and source-verification notes
- `data/csv/` — synthetic CSV starter data
- `data/staging/` — optional staging/import working files
- `database/` — SQL and PL/SQL implementation organized by task
- `scripts/` — helper scripts
- `screenshots/` — evidence screenshots

## Suggested implementation order
1. Review proposal and confirm scope with instructor.
2. Complete restricted Phase I independently.
3. Profile the CSV data and finalize requirements.
4. Create normalized Oracle tables and constraints.
5. Import and validate sample data.
6. Implement procedures, functions, cursors, packages, triggers, and exception handling.
7. Test with valid, invalid, duplicate, and boundary cases.
8. Capture screenshots and update documentation.

## CSV import order
1. collection_points.csv
2. waste_categories.csv
3. recycling_facilities.csv
4. waste_collections.csv
5. transport_assignments.csv
6. recycling_records.csv

See `data/csv/README_IMPORT.txt` for relationships and import notes.
