build:
	docker build -t "anrg/swarmdag" .

push:
	docker push "anrg/swarmdag"

reset-testnet:
	sudo rm -rf build/*
	tendermint testnet --v 2 --o ./build --populate-persistent-peers --starting-ip-address 172.17.0.2

.PHONY: build push