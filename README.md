## Candor Api OpenAPI Specifications

This repository hosts the OpenAPI specifications and Swagger UI for the Candor Api. 

## Local browsing/editing

You can view and run this locally using a local static file server. Some examples include:

- [lite-server](https://github.com/johnpapa/lite-server) (can auto reload)

    ```sh
    npx lite-server
    ```

- [dotnet-serve](https://github.com/natemcmaster/dotnet-serve)

    ```sh
    dotnet tool install --global dotnet-serve
    dotnet serve
    ```

## Changelog

### v0.13.0
- Added LOS Callback for Candor Result.
- Update Swagger UI to v3.49.0

### v0.12.0
- Change `investor` to an array and rename to `investors`
- Update Swagger UI to v3.48.0

### v0.11.1
- Fix invalid example
- Fixed OpenAPI linting using Spectral
- Updated token Urls

### v0.11.0
- Add response object to ICR DocumentsAvailable callback
- Change Decision models of `id` to a named id: `loanId`, `conditionId`
- Added `filename` back to Decision `inputDocuments`
- Added new ICR status codes
- Updated Document status codes across all entities

### v0.10.0
- Change `ezToClose` to `insuranceScore`
- Decision documents to/from all have id, bucket, path, and no filename
- Add `parentId` to `documentsProcessed`
- Changed casing of Decisions' `sessionid`
- Added required Decisions' property `outputtype: "Json"`
- Changed input/output/documentsProcessed `id` to `fileId`, and changed `parentId` to `parentFileId`

### v0.9.1
- Updated `FNM32` to instead be `URLA`: Universal Residential Loan Application

### v0.9.0
- Added a way for an ICR to report that a previously processed output file has been marked as deleted and should not be considered for further processing
- Update Swagger UI to v3.46.0

### v0.8.1
- Fixed the `$.outputDocuments.path` examples for Decisions' Process Loan Documents
- Update Swagger UI to v3.45.1

### v0.8.0
- Changed ICR file download URL structure. Consumers shouldn't be affected by this change as the full proper URL is provided to them in the `DocumentsAvailable` callback.
- Fixed misspelling of `FNM32`
- Updated Swagger UI to v3.45.0

### v0.7.0
- Allow ability to overwrite previously uploaded document
- Send filename to Decisions in `inputDocuments` and `outputDocuments`

### v0.6.0
- Added header authentication option to ICR callback registration

### v0.5.0
- Renamed the term "file" to "document" in relation to documents associated with a loan to avoid the confusion with the term "loan file" (the overall loan application file)

### v0.4.0
- Added enum values and descriptions
- Fixed some required fields
- Upper cased the `responseType` values and clarified how this controls the response of the process loan request
- Added description to Download Document endpoint
- Added recommendation for usable characters in the Document Id

### v0.3.0
- initial publish