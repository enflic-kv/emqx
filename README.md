# EMQX powered by compose

EMQX is an open-source, highly scalable, and distributed MQTT messaging broker for the Internet of Things (IoT) and real-time applications. It supports various IoT protocols, including MQTT, MQTT-SN, CoAP, and LwM2M, and it is designed to handle millions of concurrent connections and messages with low latency and high reliability. It also provides clustering and load balancing capabilities, which allows for horizontal scaling and better fault tolerance.

Compared to other MQTT brokers, such as Mosquitto, EMQX offers several benefits, such as higher scalability, better performance, and more advanced features.  Additionally, EMQX has an intuitive web-based management dashboard, which simplifies configuration, monitoring, and troubleshooting tasks.

## Requirements

* docker >= 17.12.0+
* docker-compose

## Quick Start

1. Install [docker-compose](https://docs.docker.com/compose/install/) on the docker host.
1. Clone this repo on the docker host.
1. Navigate to the directory using  `cd emqx`
1. Optionally, change default credentials in the `.env` file.
1. Run the following command from the root:

    ```bash
    docker-compose up -d
    ```

1. To stop the app, run the following command from the root of the cloned repo:

    ```bash
    docker-compose down
    ```

## Environments

This Compose file contains the following environment variables:

| Variables | Default |
| --------- | -------- |
| IMAGE_VERSION | latest |
| CONTAINER_NAME | emqx-container |
| MQTT_PORT | 1883 |
| UI_PORT | 18083 |
| EXTERNAL_NETWORK | homelab-network |
