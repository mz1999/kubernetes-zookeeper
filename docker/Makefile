VERSION=3.6.3
PROJECT_ID=mz1999
PROJECT=${PROJECT_ID}

all: build

build:
	docker build --pull -t ${PROJECT}/kubernetes-zookeeper:${VERSION} .

push: build
	gcloud docker -- push ${PROJECT}/kubernetes-zookeeper:${VERSION}

.PHONY: all build push
