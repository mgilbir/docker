all: build push

build:
	docker build -t mgilbir/golang-musl:1.8.0 .

push:
	docker push mgilbir/golang-musl:1.8.0
	docker tag mgilbir/golang-musl:1.8.0 mgilbir/golang-musl:latest

.PHONY: build push
