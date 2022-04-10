open --background -a Docker
k3d cluster create newrelic-learn

kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

brew install argocd

kubectl create namespace production
