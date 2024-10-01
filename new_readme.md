# AcuityPPM API Documentation

Welcome to the AcuityPPM API documentation. This guide provides detailed information on how to interact with the various endpoints of the AcuityPPM API.

## Table of Contents

- [AcuityPPM API Documentation](#acuityppm-api-documentation)
	- [Table of Contents](#table-of-contents)
	- [Introduction](#introduction)
	- [Authentication](#authentication)
	- [Endpoints](#endpoints)
	- [Support](#support)
	- [FAQ](#faq)

## Introduction

The AcuityPPM API allows you to interact with AcuityPPM's project portfolio management system programmatically. This API provides endpoints to retrieve and manipulate data, enabling you to integrate AcuityPPM's functionality into your applications.

## Authentication

To access the AcuityPPM API, you need an API keys. You can obtain this keys from your AcuityPPM **support**. Include the API keys in the headers of your requests.

- [Auth for list scope](1)
- [Auth for record scope](2)

## Endpoints

  - [Scope List](api_list.md)
  - [Scope Record](api_record.md)


## Support

At the moment, we have covered some parts of the API. It is also possible that some columns are not in the response that you need if you need more columns in the response then please reach out to `Acuity Support` (support@acuityppm.com) and will try and assist you. 

## FAQ

Q: Can I get list of the projects? <br>
A: You can get list of the projects see the **Endpoints -> Scope List.**

Q: Can I get/create/update a project? <br>
A: You can do that see the **Endpoints -> Scope Record.**

Q: How can I obtain an API key to get List? <br>
A: You can obtain an API key from your AcuityPPM Project Information Page.

Q: What should I do if I encounter a 401 Unauthorized error?
A: Ensure that your API key is included in the request header and is correct.

Q: Can I request additional columns in the API response?
A: Yes, if you need additional columns, please contact Acuity Support at support@acuityppm.com.
