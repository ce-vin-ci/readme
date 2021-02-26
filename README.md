# notes

![archi](ce-vin-ci.png?raw=true "Architecture")

firebase : projet "bulle étanche", avec dedans des applis (= site pour un projet web).

projet vin.fr
appli (= site) vin.fr
	domaine vin.fr
		> entête à mettre dans entête ovh
appli (= site) quizz.vin.fr
	domaine quizz.vin.fr
		> entête à mettre dans entête ovh

existe entête DNS pour les mails pour rediriger contact@vin.fr pour rediriger vers a.vergnaud@gmail.com

https://docs.ovh.com/fr/emails/guide-des-redirections-emails/

+ elasticmail
pas un client smtp
code pour envoyer un email : dans elastic mail donne un entete, elastic offre api REST
si on veut un webmail : plus cher

newsletter popup...

GatsbyJS PWA pour la partie front, blog. workbox cli scanne les static et les ajoute dans le service js pour avoir tout en offline

ReactJS PWA pour la partie quizz

le blog et le quizz sont dans strapi / cloud.mongodb.com ET cloudinary pour les files upload
hébergement d'images ...

firebase FAS

page facebook !!!

google analytics

entête OGP <head> HTML ! pour twitter ou facebook qui alimentent des vignettes dans les tweets

# CD contrib

curl -H "Authorization: token <YOUR_GITHUB_TOKEN>" \
    --request POST \
    --data '{"event_type": "<YOUR_EVENT_TYPE>"}' \
    https://api.github.com/repos/<YOUR_GITHUB_USER>/<YOUR_GITHUB_REPO>/dispatches

