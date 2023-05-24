# argocd-demo
Sync-wave-testing

argocd app create guestbook --repo https://github.com/pramachandran04/argocd-demo.git --path guestbook --dest-server https://kubernetes.default.svc --dest-namespace guestbook

argocd app create backend-app --repo https://github.com/pramachandran04/argocd-demo.git --path guestbook --dest-server https://kubernetes.default.svc --dest-namespace backend-app

argocd app create frontend-app --repo https://github.com/pramachandran04/argocd-demo.git --path guestbook --dest-server https://kubernetes.default.svc --dest-namespace frontend-app

argocd app create sync-wave --repo https://github.com/pramachandran04/argocd-demo.git --path guestbook --dest-server https://kubernetes.default.svc --dest-namespace sync-wave
