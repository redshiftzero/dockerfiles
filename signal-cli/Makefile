.PHONY: default build run

default: build run

build:
	docker build -t signal-cli .

run:
	docker run -it --name signal-cli \
	  -v ~/.config/signal:/root/.config/signal \
		--rm signal-cli
