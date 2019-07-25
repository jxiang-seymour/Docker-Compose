SHELL = /bin/bash -o pipefail

include .env

ROOT_DIR = $(CURDIR)
DOCKER_IMAGE_DIR = $(ROOT_DIR)/image

rebuild-all:  rebuild-jenkins

rebuild-jenkins:
	cd $(ROOT_DIR) && docker-compose rm -sf "jenkins" && docker-compose up -d --no-deps --build "jenkins"
