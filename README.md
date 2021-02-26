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