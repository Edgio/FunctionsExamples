# Edgio Functions Examples

## Description

This repository provides example code for implementing the most common use cases on Edgio Functions. It features
examples of how to add headers to a request, change response bodies before returning them to the client, create HTML
pages from scratch to return as a response, manipulate video player manifests, and generate JSON from scratch.

Please note that as Edgio Function is in its early beta phase, we do not advise running production traffic on it yet.
We're looking for functional feedback about APIs and features our customers need.

## Prerequisites

To use this project, you must be an Edgio customer and signed up for the Edgio Functions beta. The system requirements
include Node.js v16 or higher, and a UNIX-like system (Linux or macOS). The project code is written in JavaScript.

## Setup and Installation

1. Ensure you meet the prerequisites.
2. Clone the repository to your local machine.
3. Run `npm install` in the repository directory.

## Getting Started

After setting up the project, run `npm run edgio dev` to start a local development server to test the example functions.

To deploy the project to Edgio, use the command `npm run edgio deploy`. Note that deployment to Edgio requires you to be
logged into Edgio CLI which can be done via `npm run edgio login` and following the instructions. Also, Edgio Functions
must be enabled for your team, which can be done by contacting your account manager at Edgio and signing up for the
Edgio Functions beta.

## Known Issues and Limitations

As the project is in its early beta phase, there are a few limitations. Currently

* We only support JavaScript-based code
* Each request has a 30-second (wall time) timeout limit
* Each request is limited to 50ms of CPU time
* An Edgio Function can make fetch requests only to origins defined in your property configuration
  file (`edgio.config.js`).

## Support

If you have any queries or face issues with this project, please don't hesitate to contact
the [Edgio team](https://edg.io/contact-support/).

## License

[Creative Commons Attribution 4.0 International Public License](LICENSE-CONTENT) for the documentation.

[MIT License](LICENSE-CODE) for the code.