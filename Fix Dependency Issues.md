# Fix Dependency Issues
- npm config set legacy-peer-deps false
- delete package-lock.json and node_modules
- open package.json, hover mouse on dependency number, copy the latest verion from popup
- npm i
- npm update --package-lock-only

# Deploy
- cds build --production
- mbt build -t gen --mtar mta.tar
- cf deploy gen/mta.tar