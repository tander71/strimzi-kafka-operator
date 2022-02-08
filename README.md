# strimzi-kafka-operator

Install with helm:

$ helm repo add strimzi https://strimzi.io/charts/
$ helm update
$ k create ns operators
$ k create ns kafka-project
$ helm -n operators install strimzi-kafka-operator strimzi/strimzi-kafka-operator --set watchNamespaces="{kafka-project}"

