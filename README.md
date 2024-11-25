# AcuityPPM API Documentation

Welcome to the Acuity PPM API documentation. This guide provides detailed information on how to interact with the various endpoints of the Acuity PPM API.

## Navigation

- [AcuityPPM API Documentation](#acuityppm-api-documentation)
  - [Navigation](#navigation)
  - [Authentication](#authentication)
  - [Endpoints](#endpoints)
  - [Support](#support)
  - [FAQ](#faq)

## Authentication

To access the Acuity PPM API, you need API keys. You can obtain these keys from your Acuity PPM Account Manager or by emailing support@acuityppm.com. Please include "API keys" in the header of your requests.

### Headers for Authentication Method GET

- `Domain`
- `Company-Api-Token`

### Headers for Authentication Method GET/POST/PUT

- `Domain`
- `api-auth`
- `api-token`
- `api-secret`

## Endpoints

To get the list of modules and their endpoints, click on the links below:

- [Get - List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)
- [Get/Post/Put - Record](https://github.com/AcuityPPM/APIs/blob/main/endpoints/record.md)

## Support

At the moment, we have covered some parts of the API. It is also possible that some columns are not in the response that you need. If you need more columns in the response then please reach out to `Acuity Support` (<support@acuityppm.com>) and we will try and assist you. If you have any issue please create a new issue [here](https://github.com/AcuityPPM/APIs/issues).

## FAQ

Q: Can I get a list of all the projects? <br>
A: Yes, you can get list of the projects see the **Endpoints -> Get List.**

Q: Can I get/create/update a project? <br>
A: Yes, you can do that; see the **Endpoints -> Get/Post/Put Record.**

Q: Can I get/create/update a proposal? <br>
A: Yes, you can do that; see the **Endpoints -> Get/Post/Put Record.**

Q: Where do I find the API keys? <br>
A: You can obtain an API key from your AcuityPPM Project Information page. Click on the gear icon on the right side of the screen. If you do not see the gear icon, reach out to Acuity PPM support.

Q: What should I do if I encounter a 401 Unauthorized error? <br>
A: Ensure that your API key is included in the request header and is correct.

Q: Can I request additional columns in the API response? <br>
A: Yes, if you need additional columns, please contact Acuity PPM Support at <support@acuityppm.com>.

Q: Encounter an issue? <br>
A: Please create a new issue [github issues](https://github.com/AcuityPPM/APIs/issues)
