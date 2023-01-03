# Torrent Web Client running on AKS (transmission)
Torrent Web Client running on AKS<br>
The easy way to run a Torrent Web Client in AKS to download a torrent


If you already have a cluster, you just need to run this yaml and thats it!

kubectl apply -f https://raw.githubusercontent.com/zectorpt/transmission/main/deployment.yaml

Follow the created IP with the LoadBalancer<br>
Username: transmission<br>
Password: transmission<br>

<img width="322" alt="image" src="https://user-images.githubusercontent.com/10439948/209942841-004383bf-ba0b-4af5-b36d-2302c812b4a3.png">

# How to delete everything that was created
<br>
kubectl delete deployment transmission<br>
kubectl delete service service9091<br>

# Next version
<br>
In the next version the download will be done to a stoage account

# Where is my downloads?
<br>
Your downloads are host inside the pod in the folder: /var/lib/transmission-daemon/downloads
