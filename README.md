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

v0.8.0
- Changed ICR file download URL structure. Consumers shouldn't be affected by this change as the full proper URL is provided to them in the `DocumentsAvailable` callback.
- Fixed misspelling of `FNM32`
- Updated Swagger UI to v3.45.0

v0.7.0
- Allow ability to overwrite previously uploaded document
- Send filename to Decisions in `inputDocuments` and `outputDocuments`

v0.6.0
- Added header authentication option to ICR callback registration

v0.5.0
- Renamed the term "file" to "document" in relation to documents associated with a loan to avoid the confusion with the term "loan file" (the overall loan application file)

v0.4.0
- Added enum values and descriptions
- Fixed some required fields
- Upper cased the `responseType` values and clarified how this controls the response of the process loan request
- Added description to Download Document endpoint
- Added recommendation for usable characters in the Document Id

v0.3.0
- initial publish