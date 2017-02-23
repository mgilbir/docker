all: build push

build:
	docker build -t mgilbir/golang-musl:1.7.4 .

push:
	docker push mgilbir/golang-musl:1.7.4
	docker tag mgilbir/golang-musl:1.7.4 mgilbir/golang-musl:latest

.PHONY: build push
