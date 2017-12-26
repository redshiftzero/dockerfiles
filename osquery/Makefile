.PHONY: default build run

default: build run

build:
	docker build -t osquery .

run:  # hop into osquery interactive console
	docker run -it osquery
