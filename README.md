# Express.js JSON Body Parsing Issue

This repository demonstrates a common issue encountered when using Express.js to parse JSON request bodies.  The problem arises when the request body is either empty or contains invalid JSON data.  The provided code example showcases the issue and includes a solution to handle such scenarios gracefully.

## Bug Description

The Express.js application fails to parse the request body correctly when an empty request or an invalid JSON payload is sent in a POST request.  This results in `req.body` being undefined or containing unexpected values, leading to potential errors and unexpected behavior in the application. 

## Solution

The solution involves adding a middleware function to explicitly check for empty or invalid JSON bodies before attempting to access `req.body`.

## Usage

Clone the repository and run `npm install` to install the dependencies.  You can then start the server using `node bug.js` and test the issue and solution by sending POST requests with various payloads using tools like Postman or curl.