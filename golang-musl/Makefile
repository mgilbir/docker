all: build push

build:
	docker build -t mgilbir/golang-musl:1.11.2 .

push:
	docker push mgilbir/golang-musl:1.11.2
	docker tag mgilbir/golang-musl:1.11.2 mgilbir/golang-musl:latest

.PHONY: build push
