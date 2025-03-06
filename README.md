# SQS Consumer

<div style="display: flex; flex-direction: row; justify-content: space-evenly">
  <p>
    <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
  <p>
    <a href="https://docs.aws.amazon.com/?nc2=h_ql_doc_do" target="blank"><img src="https://cdn.worldvectorlogo.com/logos/aws-sqs.svg" width="120" alt="Nest Logo" />
    </a>
  </p>
</div>
<p align="center">
  <a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
  <a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
</p>

## Resume

Your company needs to manage the payment flow efficiently.
With a high volume of deposit and withdrawal requests, you don’t want to store these transactions in the repository, but you still need to process them from there.

## Overview

Amazon **SQS (Simple Queue Service)** is a fully managed message queuing service that enables the decoupling and scaling of distributed systems asynchronously.

It acts as a middleware between services: one system places messages in the queue, and another system consumes them when ready. This helps handle traffic spikes, distribute workload among multiple consumers, and ensure message processing without data loss.

## Types of Queues

SQS provides two main types of queues:

1. **Standard Queue** – Supports high throughput and ensures at-least-once message delivery (but messages may be duplicated or arrive out of order).
2. **FIFO Queue (First-In-First-Out)** – Guarantees exactly-once processing and preserves the exact order of messages, but has a lower throughput.

## Common Use Cases

- Payment processing  
- Bulk email sending  
- Data pipeline processing  
- Asynchronous job execution  

## Project setup

```bash
pnpm install
```

## Compile and run the project

```bash
# development
$ pnpm run start

# watch mode
$ pnpm run start:dev

# production mode
$ pnpm run start:prod
```

## Run tests

```bash
# unit tests
$ pnpm run test

# e2e tests
$ pnpm run test:e2e

# test coverage
$ pnpm run test:cov
```
