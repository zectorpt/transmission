# Torrent Web Client running on AKS (transmission)
Torrent Web Client running on AKS<br>
The easy way to run a Torrent Web Client in AKS to download a torrent and after it you can delete the deployment


If you already have a cluster, you just need to run this yaml and thats it!

kubectl apply -f https://raw.githubusercontent.com/zectorpt/transmission/main/deployment.yaml

Follow the created IP with the LoadBalancer
Username: transmission
Password: transmission
