all: build push

build:
	curl -o /tmp/kubeclient.tar.gz -L https://dl.k8s.io/$(TAG)/kubernetes-client-linux-amd64.tar.gz && \
        cd /tmp && tar xvzf kubeclient.tar.gz && \
        cd - && mkdir -p tmp && \
        mv /tmp/kubernetes/client/bin/kubectl tmp/kubectl && \
        docker build -t mgilbir/kubectl:$(TAG) . && \
        rm -rf /tmp/kubernetes && rm -rf tmp

push:
	docker push mgilbir/kubectl:$(TAG)

.PHONY: build push
