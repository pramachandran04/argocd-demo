# argocd-demo
Sync-wave-testing

argocd app create sql-upgrade --repo https://github.com/pramachandran04/argocd-demo.git --path sql-upgrade --dest-server https://kubernetes.default.svc --dest-namespace sql-upgrade

argocd app create page-up --repo https://github.com/pramachandran04/argocd-demo.git --path page-up --dest-server https://kubernetes.default.svc --dest-namespace page-up

argocd app create guestbook --repo https://github.com/pramachandran04/argocd-demo.git --path guestbook --dest-server https://kubernetes.default.svc --dest-namespace guestbook

argocd app create backend-app --repo https://github.com/pramachandran04/argocd-demo.git --path backend-app --dest-server https://kubernetes.default.svc --dest-namespace backend-app

argocd app create frontend-app --repo https://github.com/pramachandran04/argocd-demo.git --path frontend-app --dest-server https://kubernetes.default.svc --dest-namespace frontend-app

argocd app create sync-wave --repo https://github.com/pramachandran04/argocd-demo.git --path sync-wave --dest-server https://kubernetes.default.svc --dest-namespace sync-wave

argocd app delete guestbook 
argocd app delete backend-app 
argocd app delete frontend-app 
argocd app delete sync-wave 