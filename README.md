# rethinkdb-with-docker-k8s
This project is to build a simple rethinkdb docker image with k8s for running a rethinkdb cluster on Google Cluster Engine.

1. push our docker image to some registry container.
2. In this two files (Statefulset and replicationController) ymls replace in property image: docker image for our docker image that you put on registry.
3. Change in pvc file the property pdName to ours disk, for create a disk go to Google Persistent Disk.
4. Deploy first pvc yml for create a volume to your pods.
