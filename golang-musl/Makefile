all: build push

build:
	docker build -t mgilbir/golang-musl:1.10.5 .

push:
	docker push mgilbir/golang-musl:1.10.5
	docker tag mgilbir/golang-musl:1.10.5 mgilbir/golang-musl:latest

.PHONY: build push
