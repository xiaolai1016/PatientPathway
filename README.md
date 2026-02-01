Install Synthea
Clone the repository
git clone https://github.com/synthetichealth/synthea.git
cd synthea
Build Synthea
./gradlew build check test
Generate Synthetic Data
./run_synthea -p 3000 -m mental_health California

To get data exported to CSV, change csv export to exporter.csv.export = true in the file /YourPath/synthea/src/main/resources/synthea.properties
to get CSV output with header exporter.csv.append_mode = false
to get CSV output without header exporter.csv.append_mode = ture

Also can turn off JSON output by changing fhir export to exporter.fhir.export = false.
