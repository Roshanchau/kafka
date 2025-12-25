# Kafka Test Repo

This repository demonstrates a simple Kafka setup using Node.js, featuring a producer and consumer example with the `node-rdkafka` library.

## Features
- **Producer**: Publishes messages to a Kafka topic.
- **Consumer**: Subscribes to a Kafka topic and logs incoming messages.

## Prerequisites
- [Node.js](https://nodejs.org/) installed
- [Kafka](https://kafka.apache.org/) running locally (default broker: `localhost:9092`)

## Installation
1. Clone the repository:
	```sh
	git clone <repo-url>
	cd kafka-test
	```
2. Install dependencies:
	```sh
	npm install
	```

## Usage

### Start Kafka Broker
Ensure your Kafka broker is running on `localhost:9092` using `docker-compose up -d`.

### Run the Producer
Edit `publisher.js` to set your topic name (default: `'topic'`). Then run:
```sh
node publisher.js
```

### Run the Consumer
Edit `consumer.js` to set your topic name (default: `'customer-created'`). Then run:
```sh
node consumer.js
```

## Dependencies
- [node-rdkafka](https://www.npmjs.com/package/node-rdkafka )

## File Overview
- `publisher.js`: Kafka producer example
- `consumer.js`: Kafka consumer example
- `package.json`: Project dependencies

## Notes
- Make sure the topic exists in your Kafka broker before running the producer/consumer.
- You can change topic names in the respective JS files as needed.

## License
MIT
