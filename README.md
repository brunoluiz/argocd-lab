```
brew install argocd
argocd app create root \
    --dest-namespace argocd \
    --dest-server https://kubernetes.default.svc \
    --repo https://github.com/brunoluiz/argocd-lab.git \
    --path envs/sputnik
argocd app sync root --prune
```
