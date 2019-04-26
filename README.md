# rethinkdb-with-docker-k8s
This project is to build a simple rethinkdb docker image with k8s for running a rethinkdb cluster on Google Cluster Engine.

1. push docker image to some registry container.
2. In this two files (Statefulset and replicationController) change property image.
3. Change in pvc file the property pdName, for create a disk go to Google Persistent Disk.
4. Deploy first pvc for create a volume to your pods.
