# Edge Functions Examples

## Description

This repository provides example code for implementing the most common use cases on Edge Functions. It features
examples of how to add headers to a request, change response bodies before returning them to the client, create HTML
pages from scratch to return as a response, manipulate video player manifests, and generate JSON from scratch.

## Prerequisites

To use this project, you must be an Edgio customer and signed up for the Edge Functions. The system requirements
include Node.js v16 or higher, and a UNIX-like system (Linux or macOS). The project code is written in JavaScript.

## Setup and Installation

1. Ensure you meet the prerequisites.
2. Clone the repository to your local machine.
3. Run `npm install` in the repository directory.
4. Update the `team` parameter in `edgio.config.js` file to match your Edgio console team slug.

## Getting Started

After setting up the project, run `npm run edgio dev` to start a local development server to test the example functions.

To deploy the project to Edgio, use the command `npm run edgio deploy`. Note that deployment to Edgio requires you to be
logged into Edgio CLI which can be done via `npm run edgio login` and following the instructions.
This project deploys to `edge-functions-sandbox` team, you must be a member of that team to deploy or you can change
the team parameter in `edgio.config.js` file but the Edge Functions must be enabled for your team, which can be done by
contacting your account manager at Edgio and signing up for the  Edge Functions.

## Known Issues and Limitations

Currently

* We only support JavaScript-based code
* Each request has a 30-second (wall time) timeout limit
* Each request is limited to 50ms of CPU time
* Each request is limited to 2MB of memory
* An Edgio Function can make fetch requests only to origins defined in your property configuration
  file (`edgio.config.js`).

We're looking forward to feedback from our customers about these limitations and how we can improve the product.

## Support

If you have any queries or face issues with this project, please don't hesitate to contact
the [Edgio team](https://edg.io/contact-support/).

## License

[Creative Commons Attribution 4.0 International Public License](LICENSE-CONTENT) for the documentation.

[MIT License](LICENSE-CODE) for the code.
