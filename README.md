# Notifications Control

This Node.js application uses NestJS, a framework for building efficient, scalable server-side applications, Jest, a popular JavaScript testing framework, and Prisma, a modern data layer for Node.js and TypeScript.

## Installation

To install this application and its dependencies, run the following command:

```bash
$ npm install
```

## Testing

To run the test suite for this application, use the following command:

```bash
$ npm run test
```

This will run all of the tests defined in the test directory using Jest.

## Usage

To start the application, use the following command:

```bash
$ npm run start:dev
```

This will start the application and make it available at http://localhost:3000/.

To control notifications, you can send HTTP requests to the following endpoints:

- `POST /notifications`: This endpoint allows you to create a new notification.
- `GET /notifications/from/:recipientId`: This endpoint allows you to retrieve notifications from an recipient.
- `GET /notifications/count/from/:recipientId`: This endpoint allows you to count notifications from an recipient.
- `PATCH /notifications/:id/read`: This endpoint allows you to read an notification by its ID.
- `PATCH /notifications/:id/unread`: This endpoint allows you to unread an notification by its ID.
- `PATCH /notifications/:id/cancel`: This endpoint allows you to cancel a notification by its ID.

## Data Storage

This application uses Prisma as its data layer, which provides a secure and efficient way to store and retrieve data. You can find the schema for the data model in the `prisma/schema.prisma` file.

For testing purposes, this application also includes an in-memory notifications repository. This repository is used to store notifications while running the test suite, and is not used in the production version of the application.

## License

This project is licensed under the MIT License.