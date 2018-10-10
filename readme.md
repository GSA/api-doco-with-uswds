** Rough Draft In Progress **

# API Documentation Template - simple, accessible and using USWDS

This is an updated version of the GSA API Documentation template. You can see a working version of it here: [https://ryandaydev.github.io/api-doco-with-uswds/](https://ryandaydev.github.io/api-doco-with-uswds/).

It has the following improvements from the existing GSA API documentation template:
- Tested for [Section 508 accessibility](https://section508.gov/)
- Uses [U.S. Web Design System](https://designsystem.digital.gov/). Specifically the [Documentation Template](https://designsystem.digital.gov/page-templates/#documentation-page)
- Uses [Open API Specification (OAS) 3.0](https://github.com/OAI/OpenAPI-Specification)


![alt text](other/screenshot_of_doco_template.png "Screenshot of API documentation template with Prototype City Pairs API")


## Dependencies
- Swagger UI v 3.18.3 (with customizations) - https://github.com/swagger-api/swagger-ui/tree/v3.18.3
- USWDS 1.6.8 - https://designsystem.digital.gov/download/

## Customization for Accessbility
- For section 508 accessibility, edits have been made directly to the minified [swagger-ui-bundle.js](swagger-ui-bundle.js) file. This is a workaround, but the best situation would be for those changes to be implemented in the SwaggerUI.
- To see the original violations before the customization, view the [original AMP report](other/AMP_report_original.pdf) and [detail](other/AMP_violations_before_customization.xls).
- To see the result of the customizations, view the [updated report](other/AMP_report_after_customization.pdf)

## Running locally  

Because this uses HTML and JavaScript, the files can be opened locally in the browser. However, to run the Swagger UI on page 3, it will need to be run on a web server.

An example of a simple local web server on a Mac is to run the following command in the root directory:

`python -m http.server`
