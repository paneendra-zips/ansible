# Ansible Role: RabbitMQ

Installs RabbitMQ on Linux.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    rabbitmq_daemon: rabbitmq-server
    rabbitmq_state: started
    rabbitmq_enabled: true

Controls the RabbitMQ daemon's state and whether it starts at boot.

    rabbitmq_version: "3.6.16"

    rabbitmq_deb: "rabbitmq-server_{{ rabbitmq_version }}-1_all.deb"
    rabbitmq_deb_url: "https://packagecloud.io/rabbitmq/rabbitmq-server/packages/{{ ansible_distribution | lower }}/{{ ansible_distribution_release }}/{{ rabbitmq_deb }}/download"

(Debian/Ubuntu only) Controls the .deb to install.

