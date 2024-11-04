# timekube
timekube is a project for creating helm-chart for nginx webserver which shows current time.

original task:
using any available cloud provider, bring up the container with nginx. It is necessary for the container to write the current date-time to a file in the storage once every 30 seconds. It is necessary that in the scenario where the container is dropped and removed, kubernetes itself raises a new container with the same storage, and the process continues further. The page with the file should open on the Internet. The format of writing to the file: an arbitrary string, not sewn into the program code of the container plus a date in the format yyyy-mm-dd-HH:mm:ss: “bla-bla-bla 2024-01-25-10:20:30”.

I used helm chart with deployment.yaml, pvc.yaml and service.yaml for this project. the main values are stored in values.yaml.
