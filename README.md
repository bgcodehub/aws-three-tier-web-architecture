# AWS Three-Tier Web Architecture Project

## Table of Contents

1. [Introduction](#introduction)
2. [Target Audience](#target-audience)
3. [Prerequisites](#prerequisites)
4. [Architecture Overview](#architecture-overview)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Contribution Guidelines](#contribution-guidelines)

## Introduction

Welcome to my personal project on AWS Three-Tier Web Architecture. In this project, I've built an intricate, three-tier web architecture leveraging AWS services. This project entails the detailed construction and configuration of essential network, security, application, and database components necessary to execute this architecture in a scalable and readily available manner.

## Target Audience

This project primarily targets individuals with a technical inclination. It's assumed that you possess foundational knowledge of AWS services including, but not limited to VPC, EC2, RDS, S3, ELB, and are acquainted with the AWS Console.

## Prerequisites

Before diving into this project, make sure you have:

- An active AWS account. If you lack one, follow the instructions [here](https://portal.aws.amazon.com/billing/signup#/start) and click on “Create an AWS Account” button in the top right corner.
- An IDE or text editor of your choice.

## Architecture Overview

The following diagram illustrates the architecture used in this project:

![3TierArch](https://github.com/bgcodehub/aws-three-tier-web-architecture/assets/97926762/e612d572-e705-4247-a2b6-34a4372319ff)

In this architecture, a client-facing Application Load Balancer directs client traffic to our web tier EC2 instances. The web tier, equipped with Nginx web servers, serves a React.js website and redirects API calls to the application tier’s internal load balancer. The internal load balancer subsequently directs this traffic to the application tier, powered by Node.js. The application tier interacts with a multi-AZ Aurora MySQL database, manipulating data and returning it to the web tier. I've implemented load balancing, health checks, and auto-scaling groups at each layer to ensure the architecture's availability.

## Installation

Detailed installation instructions can be found on my personal website, [briangaleano.com](https://www.briangaleano.com).

## Usage

For a complete walkthrough on how to use this project, please visit [briangaleano.com](https://www.briangaleano.com).

## Contribution Guidelines

If you'd like to contribute to this project, follow the steps below:

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Your contributions to making this project more efficient and effective are greatly appreciated!

