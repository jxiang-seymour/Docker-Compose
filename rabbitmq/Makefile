SHELL = /bin/bash -o pipefail


ROOT_DIR = $(CURDIR)

rebuild-all:  rebuild-rabbit1

rebuild-rabbit1:
	cd $(ROOT_DIR) && docker-compose rm -sf "rabbit1" && docker-compose up -d --no-deps --build "rabbit1"
