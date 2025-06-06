# ⚠️Important Vulnerabilities (CVSS > 8)⚠️
* ⚔️ Critical Fortinet flaws now exploited in Qilin ransomware attacks
* 🔒 CVE-2025-47601 - MaxiBlocks Missing Authorization Privilege Escalation
* 🔒 CVE-2025-5799 - Tenda AC8 Stack-Based Buffer Overflow Vulnerability
* 🔒 CVE-2025-5798 - Tenda AC8 Stack-Based Buffer Overflow Vulnerability
* 🔒 CVE-2025-5795 - Tenda AC5 Buffer Overflow Vulnerability
* 🔒 CVE-2025-5794 - Tenda AC5 PPTP User List Buffer Overflow Vulnerability
* 🔑 CVE-2025-2766 - 70mai A510 Default Password Authentication Bypass
* 🔒 CVE-2025-5793 - TOTOLINK EX1200T HTTP POST Request Handler Buffer Overflow Vulnerability
* 💻 How Falcon Next-Gen SIEM Protects Enterprises from VMware vCenter Attacks (CVE-2023-34048)
* 🛠️ Unpatched XSS Vulnerability in Jenkins Gatling Plugin Puts Users at Risk (CVE-2025-5806)
* 📢 CISA Alert: Critical Vulnerabilities Found in CyberData SIP Emergency Intercom Devices
* 📁 Microsoft shares script to restore inetpub folder you shouldn’t delete (CVE-2025-21204)

## Table of Contents
* [Category : VULNERABILITIES](#category---vulnerabilities)
    * [Microsoft rappelle l'importance du dossier 'inetpub' pour atténuer la vulnérabilité CVE-2025-21204](#microsoft-appelle-limpornce-du-dossier-inetpub-pour-attnuer-la-vulnrabilit-cve-2025-21204)
    * [Vulnérabilité d'escalade de privilèges par autorisation manquante dans MaxiBlocks (CVE-2025-47601)](#vulnrabilit-descalade-de-privilges-par-autorisation-manque-dans-maxiblocks-cve-2025-47601)
    * [Vulnérabilités critiques par débordement de tampon dans les routeurs Tenda AC8 et AC5](#vulnrabilits-critiques-par-dbordement-de-tampon-dans-les-routeurs-tenda-ac8-et-ac5)
    * [Vulnérabilité de contournement d'authentification par mot de passe par défaut dans 70mai A510 (CVE-2025-2766)](#vulnrabilit-de-contournement-dauthentification-par-mot-de-passe-par-dfaut-dans-70mai-a510-cve-2025-2766)
    * [Vulnérabilité critique par débordement de tampon dans TOTOLINK EX1200T (CVE-2025-5793)](#vulnrabilit-critique-par-dbordement-de-tampon-dans-totolink-ex1200t-cve-2025-5793)
    * [Protection contre les attaques VMware vCenter exploitant CVE-2023-34048](#protection-contre-les-attaques-vmware-vcenter-exploitant-cve-2023-34048)
    * [Vulnérabilité XSS non corrigée dans le plugin Jenkins Gatling (CVE-2025-5806)](#vulnrabilit-xss-non-corrige-dans-le-plugin-jenkins-gatling-cve-2025-5806)
    * [Alert CISA : Vulnérabilités critiques dans les dispositifs CyberData SIP Emergency Intercom](#alert-cisa--vulnrabilits-critiques-dans-les-dispositifs-cyberdata-sip-emergency-intercom)
* [Category : THREATS](#category---threats)
    * [Optima Tax Relief victime du ransomware Chaos et de fuite de données](#optima-tax-relief-victime-du-ransomware-chaos-et-de-fuite-de-donnes)
    * [Kettering Health confirme une cyberattaque par le groupe ransomware Interlock](#kettering-health-confirme-une-cyberattaque-par-le-groupe-ransomware-interlock)
    * [Nouveau malware d'effacement de données PathWiper utilisé contre les infrastructures critiques ukrainiennes par des acteurs liés à la Russie](#nouveau-malware-deffacement-de-donnes-pathwiper-utilis-contre-les-infrastructures-critiques-ukrainiennes-par-des-acteurs-lis--la-russie)
    * [Exploitation des vulnérabilités Fortinet par le ransomware Qilin](#exploitation-des-vulnrabilits-fortinet-par-le-ransomware-qilin)
    * [Récompense américaine de 10 millions de dollars pour des informations sur le créateur du malware RedLine et des hackers d'État](#rcompense-amricaine-de-10-millions-de-dollars-pour-des-informations-sur-le-crateur-du-malware-redline-et-des-hackers-dtat)
    * [Le groupe ransomware Play a touché 900 organisations depuis 2022](#le-groupe-ransomware-play-a-touch-900-organisations-depuis-2022)
    * [Malware Blitz : Analyse d'une campagne via des cheats de jeu et abus de Hugging Face pour le C2](#malware-blitz--analyse-dune-campagne-via-des-cheats-de-jeu-et-abus-de-hugging-face-pour-le-c2)

## Category : VULNERABILITIES
### Microsoft rappelle l'importance du dossier 'inetpub' pour atténuer la vulnérabilité CVE-2025-21204
Microsoft a publié un script PowerShell pour aider à restaurer le dossier vide 'inetpub' créé par les mises à jour de sécurité Windows d'avril 2025, s'il a été supprimé 🤔. Ce dossier est crucial pour atténuer une vulnérabilité d'escalade de privilèges de haute gravité (CVE-2025-21204) dans Windows Process Activation, causée par un problème de résolution de lien impropre dans la pile de mise à jour Windows. La suppression du dossier rend le système à nouveau vulnérable 😟. Microsoft insiste sur le fait que ce dossier ne doit pas être supprimé, qu'IIS soit actif ou non, car il fait partie des changements visant à renforcer la protection. Un expert a démontré que des utilisateurs non-administrateurs peuvent abuser de ce dossier pour bloquer les mises à jour Windows en créant une jonction 🚫.
* Publication date : 2025/06/06
* Source : https://www.bleepingcomputer.com/news/microsoft/microsoft-shares-script-to-restore-inetpub-folder-you-shouldnt-delete/
* 🔗 CVE : [CVE-2025-21204](https://nvd.nist.gov/vuln/detail/CVE-2025-21204)
* 📦 CVE Impacted Product : Microsoft Windows Update Stack, Microsoft Internet Information Server (IIS)
* 💥 CVSS : N/A (signalé comme haute gravité)
* 🕴️ Threat Actor : N/A
* 📂 FILE_NAME : C:\Inetpub
* 💡 Security recommandations : Ne supprimez pas le dossier `C:\Inetpub`. Si vous l'avez supprimé, recréez-le manuellement en installant IIS via le panneau "Activer ou désactiver des fonctionnalités Windows", puis désinstallez IIS si nécessaire (le dossier restera). Appliquez les mises à jour de sécurité Microsoft d'avril 2025.

### Vulnérabilité d'escalade de privilèges par autorisation manquante dans MaxiBlocks (CVE-2025-47601)
Une vulnérabilité d'autorisation manquante a été découverte dans MaxiBlocks, permettant une escalade de privilèges 🛡️➡️🔑.
* Publication date : 2025/06/07
* Source : https://cvefeed.io/vuln/detail/CVE-2025-47601
* 🔗 CVE : [CVE-2025-47601](https://nvd.nist.gov/vuln/detail/CVE-2025-47601)
* 📦 CVE Impacted Product : MaxiBlocks : jusqu'à 2.1.0 inclus.
* 💥 CVSS : 8.8
* 🔥 EPSS : N/A
* 💡 Security recommandations : Mettre à jour le plugin MaxiBlocks vers une version corrigée dès que disponible.

### Vulnérabilités critiques par débordement de tampon dans les routeurs Tenda AC8 et AC5
Plusieurs vulnérabilités classées comme critiques par débordement de tampon ont été découvertes dans les routeurs Tenda AC8 et AC5 📶💣. Ces failles affectent différentes fonctions et fichiers et peuvent être exploitées à distance. Des exploits publics sont disponibles ⚠️.
* Publication date : 2025/06/06
* Source : https://cvefeed.io/vuln/detail/CVE-2025-5799 , https://cvefeed.io/vuln/detail/CVE-2025-5798 , https://cvefeed.io/vuln/detail/CVE-2025-5795 , https://cvefeed.io/vuln/detail/CVE-2025-5794
* 🔗 CVE : [CVE-2025-5799](https://nvd.nist.gov/vuln/detail/CVE-2025-5799), [CVE-2025-5798](https://nvd.nist.gov/vuln/detail/CVE-2025-5798), [CVE-2025-5795](https://nvd.nist.gov/vuln/detail/CVE-2025-5795), [CVE-2025-5794](https://nvd.nist.gov/vuln/detail/CVE-2025-5794)
* 📦 CVE Impacted Product : Tenda AC8 16.03.34.09, Tenda AC5 1.0/15.03.06.47.
* 💥 CVSS : 8.8 pour chaque CVE
* 🔥 EPSS : N/A
* 💡 Security recommandations : Mettre à jour le firmware des routeurs Tenda concernés vers les versions corrigées dès que disponibles. Isoler les appareils vulnérables du réseau Internet public si une mise à jour n'est pas immédiatement possible.

### Vulnérabilité de contournement d'authentification par mot de passe par défaut dans 70mai A510 (CVE-2025-2766)
Une vulnérabilité de contournement d'authentification par mot de passe par défaut a été identifiée dans le 70mai A510 (ZDI-CAN-24996) 🚪🔑. Cette faille permet à des attaquants à proximité du réseau de contourner l'authentification sans nécessiter de crédentiels et d'exécuter potentiellement du code arbitraire en tant que root 🚀.
* Publication date : 2025/06/06
* Source : https://cvefeed.io/vuln/detail/CVE-2025-2766
* 🔗 CVE : [CVE-2025-2766](https://nvd.nist.gov/vuln/detail/CVE-2025-2766)
* 📦 CVE Impacted Product : 70mai A510.
* 💥 CVSS : 8.8
* 🔥 EPSS : N/A
* 💡 Security recommandations : Changer le mot de passe par défaut du dispositif 70mai A510. Rechercher et appliquer toute mise à jour de firmware disponible.

### Vulnérabilité critique par débordement de tampon dans TOTOLINK EX1200T (CVE-2025-5793)
Une vulnérabilité critique par débordement de tampon a été découverte dans le TOTOLINK EX1200T version 4.1.2cu.5232_B20210713 📶💥. Cette faille affecte le composant HTTP POST Request Handler et peut être exploitée à distance via la manipulation de l'argument `service_type`. L'exploit a été divulgué publiquement ⚠️.
* Publication date : 2025/06/06
* Source : https://cvefeed.io/vuln/detail/CVE-2025-5793
* 🔗 CVE : [CVE-2025-5793](https://nvd.nist.gov/vuln/detail/CVE-2025-5793)
* 📦 CVE Impacted Product : TOTOLINK EX1200T 4.1.2cu.5232_B20210713.
* 💥 CVSS : 8.8
* 🔥 EPSS : N/A
* 💡 Security recommandations : Mettre à jour le firmware du TOTOLINK EX1200T vers une version corrigée dès que disponible. Isoler l'appareil du réseau Internet public si une mise à jour n'est pas immédiatement possible.

### Protection contre les attaques VMware vCenter exploitant CVE-2023-34048
CrowdStrike discute des méthodes pour protéger les instances VMware vCenter contre les attaques 🛡️, en particulier celles exploitant la vulnérabilité critique d'exécution de code à distance CVE-2023-34048 (CVSS 9.8) qui a été activement exploitée début 2024 🚨. Des scénarios d'attaque sont décrits, incluant l'établissement de persistance via la création de machines virtuelles "rogues" à partir d'ISO ou le ciblage de contrôleurs de domaine virtualisés pour voler des informations d'identification en montant leurs disques virtuels (utilisant des outils comme Impacket/secretsdump.py) 😈💾. L'article met l'accent sur la détection de ces activités en utilisant un SIEM de nouvelle génération.
* Publication date : 2025/06/07
* Source : https://www.crowdstrike.com/en-us/blog/falcon-next-gen-siem-protects-against-vmware-vcenter-attacks/
* 🔗 CVE : [CVE-2023-34048](https://nvd.nist.gov/vuln/detail/CVE-2023-34048)
* 📦 CVE Impacted Product : VMware vCenter Server
* 💥 CVSS : 9.8
* 🔥 EPSS : N/A
* 👤 Threat Actor : N/A (Acteurs exploitant la vulnérabilité)
* 🏹 Threat Target : Instances VMware vCenter, Contrôleurs de domaine virtualisés
* 🔧 Threat Tools : Impacket, secretsdump.py
* 💡 Security recommandations : Appliquez immédiatement les correctifs pour CVE-2023-34048 si ce n'est pas déjà fait. Surveillez les logs vCenter pour détecter les activités suspectes (téléchargement/upload d'ISO, création de VM, montage de disques virtuels de systèmes critiques comme les DCs). Mettez en place des règles SIEM pour identifier ces schémas d'attaque.

### Vulnérabilité XSS non corrigée dans le plugin Jenkins Gatling (CVE-2025-5806)
Une vulnérabilité de Cross-Site Scripting (XSS) de haute gravité (CVSS 8.0) a été découverte dans le plugin Jenkins Gatling version 136.vb_9009b_3d33a_e et les versions antérieures 🛠️🐞. Cette faille permet de contourner les protections Content-Security-Policy (CSP) de Jenkins, ouvrant la porte à l'injection de JavaScript malveillant si les utilisateurs peuvent modifier ou télécharger du contenu de rapport Gatling ✍️ Scripting malveillant. L'exploitation pourrait permettre l'accès à des secrets, l'exécution d'actions, la modification de configuration ou le vol de crédentiels 🔑💻.
* Publication date : 2025/06/07
* Source : https://securityonline.info/unpatched-xss-vulnerability-in-jenkins-gatling-plugin-puts-users-at-risk-cve-2025-5806/
* 🔗 CVE : [CVE-2025-5806](https://nvd.nist.gov/vuln/detail/CVE-2025-5806)
* 📦 CVE Impacted Product : Jenkins Gatling Plugin version 136.vb_9009b_3d33a_e et versions antérieures.
* 💥 CVSS : 8.0
* 🔥 EPSS : N/A
* 💡 Security recommandations : Limitez les utilisateurs autorisés à modifier ou télécharger du contenu de rapport dans Jenkins. Recherchez une version corrigée du plugin Gatling et mettez à jour dès que possible.

### Alert CISA : Vulnérabilités critiques dans les dispositifs CyberData SIP Emergency Intercom
CISA a émis une alerte concernant plusieurs vulnérabilités critiques (CVSS jusqu'à 9.8) affectant les dispositifs CyberData SIP Emergency Intercom (Modèle 011209) 📢🚨. Découvertes par Claroty Team82, ces failles pourraient permettre à des attaquants distants d'obtenir un accès non autorisé, d'exécuter du code arbitraire, de divulguer des informations sensibles ou de perturber la disponibilité du système 🔌☠️ Confidentialité, Intégrité, Disponibilité. Bien qu'aucune exploitation publique ne soit actuellement confirmée, la sévérité élevée représente un risque sérieux pour les systèmes de communication critiques s'ils ne sont pas corrigés 😟.
* Publication date : 2025/06/07
* Source : https://securityonline.info/cisa-alert-critical-vulnerabilities-found-in-cyberdata-sip-emergency-intercom-devices/
* 📦 CVE Impacted Product : CyberData SIP Emergency Intercom (Modèle 011209).
* 💥 CVSS : jusqu'à 9.8
* 🔥 EPSS : N/A
* 💡 Security recommandations : Recherchez les mises à jour de firmware ou les correctifs de CyberData pour le Modèle 011209 et appliquez-les immédiatement. Isolez les appareils vulnérables du réseau Internet public si possible.

## Category : THREATS
### Optima Tax Relief victime du ransomware Chaos et de fuite de données
L'entreprise américaine de résolution fiscale Optima Tax Relief a été victime d'une attaque par le ransomware Chaos 😈💸. Les acteurs de la menace ont exfiltré des données, qui sont maintenant divulguées 📂 Leak. Les documents fiscaux volés contiennent potentiellement des informations personnelles sensibles (numéros de sécurité sociale, adresses, etc.) pouvant être utilisées pour l'usurpation d'identité ou d'autres activités malveillantes 😟.
* Publication date : 2025/06/06
* Source : https://www.bleepingcomputer.com/news/security/tax-resolution-firm-optima-tax-relief-hit-by-ransomware-data-leaked/
* 👤 Threat Actor : Chaos ransomware
* 🏹 Threat Target : Optima Tax Relief (entreprise de résolution fiscale)
* 🔧 Threat Tools : Chaos ransomware
* 💡 Security recommandations : N/A (informations spécifiques à l'entreprise victime)

### Kettering Health confirme une cyberattaque par le groupe ransomware Interlock
Kettering Health, un réseau de santé de l'Ohio, a confirmé que le groupe ransomware Interlock a infiltré son réseau et volé des données lors d'une cyberattaque en mai 🏥😟. Le groupe a revendiqué l'attaque et publié des échantillons de données prétendument volées (941 GB), incluant des données patients, des documents de paie, et des informations sur le personnel 📁 Leak. Interlock est également associé aux attaques "ClickFix" (usurpation d'outils IT pour l'accès initial) et au déploiement d'un RAT inconnu nommé NodeSnake 🐍. Le réseau de santé travaille à rétablir les canaux de communication et a renforcé ses protocoles de sécurité 🛠️🔒.
* Publication date : 2025/06/06
* Source : https://www.bleepingcomputer.com/news/security/kettering-health-confirms-interlock-ransomware-behind-cyberattack/
* 👤 Threat Actor : Interlock ransomware group
* 🏹 Threat Target : Kettering Health (réseau de santé)
* 💃 Threat Tactic : Double Extortion (probablement, basé sur la fuite de données), Accès Initial (associé aux attaques "ClickFix"), Persistance/C2 (déploiement de RAT)
* 🔧 Threat Tools : Interlock ransomware, NodeSnake (RAT)
* 💡 Security recommandations : Renforcer la sécurité des accès initiaux (ex: authentification forte, surveillance des outils d'administration). Mettre en œuvre une segmentation réseau. Améliorer la surveillance et les contrôles d'accès.

### Nouveau malware d'effacement de données PathWiper utilisé contre les infrastructures critiques ukrainiennes par des acteurs liés à la Russie
Un nouvel effaceur de données (wiper) nommé 'PathWiper' est utilisé dans des attaques ciblées contre les infrastructures critiques en Ukraine 🇺🇦💥💾. Attribué avec une forte confiance à un groupe APT lié à la Russie, basé sur les TTPs similaires à des attaques antérieures contre l'Ukraine 🕴️🇷🇺. Les attaquants ont utilisé un outil d'administration de point d'extrémité légitime pour déployer PathWiper 🔧. Le malware cible les structures de système de fichiers NTFS (MBR, $MFT, etc.), écrasant les données avec des informations aléatoires et démontant les volumes. Il est similaire à HermeticWiper (lié au groupe russe Sandworm) mais utilise des méthodes plus précises pour identifier et corrompre les disques 📝. Le déploiement s'est fait via des fichiers BAT exécutant un VBScript malveillant (`uacinstall.vbs`) qui déposait et exécutait l'exécutable PathWiper (`sha256sum.exe`) 🤔.
* Publication date : 2025/06/06
* Source : https://www.bleepingcomputer.com/news/security/new-pathwiper-data-wiper-malware-hits-critical-infrastructure-in-ukraine/ , https://securityaffairs.com/178726/apt/russia-linked-threat-actors-targets-ukraine-with-pathwiper-wiper.html
* 👤 Threat Actor : Acteur APT lié à la Russie
* 🏹 Threat Target : Infrastructures critiques en Ukraine
* 💃 Threat Tactic : Effacement de données, Utilisation d'outils légitimes, Déploiement de malware
* 🔧 Threat Tools : PathWiper (wiper), uacinstall.vbs (VBScript), sha256sum.exe (exécutable PathWiper)
* 📂 FILE_NAME : uacinstall.vbs, sha256sum.exe
* 💡 Security recommandations : Mettez en œuvre des mesures de détection et de prévention avancées sur les points d'extrémité pour identifier les activités suspectes (exécution de scripts inhabituels, accès non standard aux structures de système de fichiers). Surveillez l'utilisation d'outils d'administration légitimes pour détecter tout abus. Maintenez des sauvegardes robustes et hors ligne des données critiques.

### Exploitation des vulnérabilités Fortinet par le ransomware Qilin
Le groupe ransomware Qilin (également suivi sous le nom de Phantom Mantis) exploite activement deux vulnérabilités Fortinet pour contourner l'authentification et exécuter du code à distance sur les appareils vulnérables ⚔️🔓. Les failles exploitées incluent CVE-2024-21762 (CVSS 9.6, RCE, déjà exploitée en tant que zero-day et ajoutée au catalogue CISA KEV) et CVE-2024-55591 (CVSS 8.8, contournement d'authentification) 🔥🚨. Le groupe, actif depuis août 2022, cible actuellement des organisations dans les pays hispanophones, mais s'attend à une expansion mondiale 🌎. Qilin utilise un modèle de double extorsion 💸📄. D'autres acteurs comme Mora_001 (potentiellement lié à LockBit) ont également exploité CVE-2024-55591 pour déployer le ransomware SuperBlack 🤝.
* Publication date : 2025/06/06
* Source : https://www.bleepingcomputer.com/news/security/critical-fortinet-flaws-now-exploited-in-qilin-ransomware-attacks/ , https://securityaffairs.com/178736/hacking/attackers-exploit-fortinet-flaws-to-deploy-qilin-ransomware.html
* 🔗 CVE : [CVE-2024-21762](https://nvd.nist.gov/vuln/detail/CVE-2024-21762), [CVE-2024-55591](https://nvd.nist.gov/vuln/detail/CVE-2024-55591), [CVE-2022-42475](https://nvd.nist.gov/vuln/detail/CVE-2022-42475), [CVE-2023-27997](https://nvd.nist.gov/vuln/detail/CVE-2023-27997)
* 💥 CVSS : CVE-2024-21762 (9.6), CVE-2024-55591 (8.8)
* 🔥 EPSS : N/A
* 👤 Threat Actor : Qilin ransomware (Phantom Mantis), Mora_001, Volt Typhoon (mentionné pour d'autres exploits Fortinet)
* 🏹 Threat Target : Organisations (actuellement pays hispanophones, puis mondial), FortiGate firewalls
* 💃 Threat Tactic : Exploitation de vulnérabilités (accès initial), Double Extorsion, Exécution de code à distance, Contournement d'authentification
* 🔧 Threat Tools : Qilin ransomware, SuperBlack ransomware, Coathanger (RAT, utilisé par Volt Typhoon)
* 🗺️ Indicator of Compromise :
    * DOMAIN: t[.]co
    * DOMAIN: bdjex2kqqopic[.]twitter[.]com
    * URL: hxxps[:]//t[.]co/BDjEX2KqqOpic[.]twitter[.]com/oRHQzzIph8
* 💡 Security recommandations : Appliquez immédiatement les correctifs pour CVE-2024-21762 et CVE-2024-55591 si ce n'est pas déjà fait. Mettez à jour tous les dispositifs Fortinet (FortiOS, FortiProxy) vers les dernières versions. Surveillez les tentatives d'exploitation et les activités suspectes sur les VPN SSL Fortinet exposés.

### Récompense américaine de 10 millions de dollars pour des informations sur le créateur du malware RedLine et des hackers d'État
Le Département d'État américain offre une récompense allant jusqu'à 10 millions de dollars pour des informations menant à l'identification ou à la localisation d'acteurs étatiques liés au malware RedLine infostealer, ainsi que sur son auteur présumé, le ressortissant russe Maxim Alexandrovich Rudometov 💰🕵️‍♂️. Rudometov est connu sous divers alias (dendimirror, alinchok, makc1901, bloodzz.fenix) et aurait géré l'infrastructure technique et les comptes crypto liés à l'opération RedLine 💻₿. La récompense vise les personnes agissant sous le contrôle d'un gouvernement étranger qui participent à des activités cyber malveillantes contre les infrastructures critiques américaines 🇺🇸🔌. En octobre 2024, la police néerlandaise, dans le cadre de l'Opération Magnus coordonnée par Eurojust, avait démantelé l'infrastructure utilisée par RedLine et META infostealers, considérés comme l'une des plus grandes plateformes de malware mondiales 🌐✋.
* Publication date : 2025/06/06
* Source : https://securityaffairs.com/178712/cyber-crime/u-s-offers-10m-bounty-for-info-on-redline-malware-creator-and-state-hackers.html
* 👤 Threat Actor : Maxim Alexandrovich Rudometov (alias dendimirror, alinchok, makc1901, bloodzz.fenix), acteurs étatiques liés à la Russie (présumé)
* 🏹 Threat Target : Infrastructures critiques américaines, millions de victimes dans le monde (pour RedLine/META)
* 💃 Threat Tactic : Vol d'informations (infostealer), Activités cyber malveillantes parrainées par l'État
* 🔧 Threat Tools : RedLine (infostealer), META (infostealer)
* 💡 Security recommandations : N/A (information de renseignement et d'enquête)

### Le groupe ransomware Play a touché 900 organisations depuis 2022
Le groupe ransomware Play a touché environ 900 organisations au cours des trois dernières années, selon un avis conjoint du FBI, de la CISA et de l'ASD's ACSC 😈📈. Actif depuis juin 2022, Play a ciblé des victimes notables comme la Ville d'Oakland, Rackspace et Royal Dirkzwager 🏙️☁️🚢. Le groupe utilise un modèle de double extorsion et contacte les victimes via des adresses email `@gmx.de` ou `@web.de` 💸📄📧. L'accès initial est souvent obtenu via des identifiants volés ou l'exploitation de vulnérabilités connues dans FortiOS, Microsoft Exchange, RDP et VPNs 🔑🔓. Plus récemment, ils ont exploité une nouvelle vulnérabilité SimpleHelp (CVE-2024-57727, RCE) 🐞. Play utilise divers outils pour la reconnaissance (AdFind, Grixba), la désactivation de sécurité (GMER, IOBit, PowerTool, scripts PowerShell) et le mouvement latéral (Cobalt Strike, SystemBC, PsExec) 🛠️🕸️. Ils volent également des identifiants (Mimikatz), élèvent les privilèges (WinPEAS) et déploient le malware via GPO, recompilant chaque binaire ransomware pour compliquer la détection 🔄 stealth.
* Publication date : 2025/06/06
* Source : https://securityaffairs.com/178702/cyber-crime/play-ransomware-group-hit-900-organizations-since-2022.html
* 🔗 CVE : [CVE-2024-57727](https://nvd.nist.gov/vuln/detail/CVE-2024-57727)
* 💥 CVSS : N/A
* 🔥 EPSS : N/A
* 👤 Threat Actor : Play ransomware group
* 🏹 Threat Target : Organisations (environ 900 victimes)
* 💃 Threat Tactic : Double Extorsion, Accès Initial (identifiants volés, exploitation de vulnérabilités), Reconnaissance, Désactivation de sécurité, Mouvement latéral, Vol d'identifiants, Escalade de privilèges, Persistance, Déploiement de ransomware
* 🔧 Threat Tools : Play ransomware, AdFind, Grixba, GMER, IOBit, PowerTool, PowerShell scripts, Cobalt Strike, SystemBC, PsExec, Mimikatz, WinPEAS
* 🗺️ Indicator of Compromise :
    * DOMAIN: web[.]de
    * DOMAIN: gmx[.]de
    * EMAIL: or@web[.]de
    * EMAIL: via@gmx[.]de
* 💡 Security recommandations : Appliquez immédiatement les correctifs pour les vulnérabilités connues, notamment CVE-2024-57727 si vous utilisez SimpleHelp. Renforcez les politiques de mot de passe et implémentez l'authentification multi-facteurs. Segmentez les réseaux. Mettez en place une surveillance réseau pour détecter les outils et TTPs utilisés par Play. Assurez-vous que les solutions de sécurité sont à jour et correctement configurées.

### Blitz Malware : Analyse d'une campagne via des cheats de jeu et abus de Hugging Face pour le C2
Un nouveau malware appelé Blitz, actif depuis 2024 et mis à jour en 2025, est distribué via des cheats pour le jeu mobile Standoff 2 tournant sur émulateur Windows (BlueStacks) 🎮👾. L'acteur derrière Blitz utiliserait le pseudo @sw1zzx_dev sur Telegram pour promouvoir et distribuer les cheats piégés 😈📢. Le malware se compose d'un téléchargeur (`ieapfltr.dll`) et d'un bot payload 🤖. L'auteur a abusé de Hugging Face Spaces, un dépôt de code AI, pour héberger les fichiers et composants de son infrastructure de C2 (Command and Control) ☁️📡. Blitz bot effectue du vol d'informations (frappe au clavier, captures d'écran) et a une fonction DoS 😈⌨️🖼️. La persistance est assurée via des entrées dans la base de registre (`UserInitMprLogonScript`, `EdgeUpdater`) ⚙️. Le bot injecte également un mineur de cryptomonnaie XMRig Monero (`xmrig.exe`) dans `explorer.exe` 💰⛏️. Le malware intègre des checks anti-sandbox/VM 🕵️‍♂️🔒. Une version antérieure de Blitz se propageait via Discord et des installeurs trojanisés, utilisant une autre URL Hugging Face (`swizxx-blitz-net.hf.space`). Bien que l'auteur ait annoncé son départ et fourni un outil de nettoyage (`cleaner.exe`), ce dernier est imparfait 🧹🐞.
* Publication date : 2025/06/06
* Source : https://unit42.paloaltonetworks.com/blitz-malware-2025/
* 👤 Threat Actor : @sw1zzx_dev (Russian speaker, présumé)
* 🏹 Threat Target : Utilisateurs de cheats de jeu pour Standoff 2 sur Windows (via BlueStacks)
* 💃 Threat Tactic : Distribution de malware (via logiciels piégés/cheats), Abus de services légitimes (Hugging Face, Telegram), Vol d'informations, Déni de service (DoS), Minage de cryptomonnaie, Persistance, Injection de processus, Anti-analyse
* 🔧 Threat Tools : Blitz downloader, Blitz bot, XMRig (Monero miner), PowerShell, cleaner.exe (outil de suppression - imparfait)
* 📂 FILE_NAME : ieapfltr.dll, Elysium_CrackBy@sw1zzx_dev.zip, Nerest_CrackBy@sw1zzx_dev.zip, elysium_android_cracked.zip, Elysium_CrackBy@sw1zzx_dev.exe, Nerest_CrackBy@sw1zzx_dev.exe, cheat_bin, cleaner.exe
* 🗺️ Indicator of Compromise :
    * DOMAIN: urlswizxx-blitz-net[.]hf[.]space
    * DOMAIN: topaste[.]rs
    * DOMAIN: channelt[.]me
    * DOMAIN: e445a00fffe335d6dac0ac0fe0a5accc-9591beae439b860-b5c7747[.]hf[.]space
    * DOMAIN: frompastebin[.]com
    * IPv4: 176[.]65[.]137[.]44
    * URL: hxxps[:]//e445a00fffe335d6dac0ac0fe0a5accc-9591beae439b860-b5c7747[.]hf[.]space/6774/[HardwareProfileGUID]
    * URL: hxxp[:]//e445a00fffe335d6dac0ac0fe0a5accc-9591beae439b860-b5c7747[.]hf[.]space/6174727A

### Analyse de la dernière vague Mirai exploitant la vulnérabilité CVE-2024-3721 dans les dispositifs TBK DVR
Une nouvelle variante du botnet Mirai exploite la vulnérabilité CVE-2024-3721 pour infecter les dispositifs TBK DVR exposés sur Internet 🌐🤖. Cette vulnérabilité permet l'exécution de commandes système sans authentification via une requête POST spécifique 🔓. Les infections ciblent spécifiquement les appareils prenant en charge les binaires ARM32 🎯. Bien que basée sur le code source de Mirai, cette variante inclut de nouvelles fonctionnalités comme le chiffrement de chaînes (RC4), des checks anti-VM et anti-émulation 🕵️‍♀️🔒. Les pays les plus touchés sont la Chine, l'Inde, l'Égypte, l'Ukraine, la Russie, la Turquie et le Brésil 🌍. Plus de 50 000 dispositifs DVR exposés ont été identifiés en ligne, offrant de nombreuses opportunités d'attaque 📈. L'objectif principal de ces bots est de mener des attaques DDoS 💥. La persistance est souvent limitée par le firmware qui ne permet pas de modifier le système de fichiers ⏳.
* Publication date : 2025/06/06
* Source : https://securelist.com/mirai-botnet-variant-targets-dvr-devices-with-cve-2024-3721/116742/
* 🔗 CVE : [CVE-2024-3721](https://nvd.nist.gov/vuln/detail/CVE-2024-3721)
* 💥 CVSS : N/A
* 🔥 EPSS : N/A
* 👤 Threat Actor : Mirai botnet operators
* 🏹 Threat Target : Dispositifs TBK DVR vulnérables
* 💃 Threat Tactic : Exploitation de vulnérabilité (accès initial), Exécution de code à distance, Formation de botnet, Attaques DDoS
* 🔧 Threat Tools : Mirai botnet variant, Exploits pour CVE-2024-3721
* 🗺️ Indicator of Compromise :
    * IPv4: 116[.]203[.]104[.]203
    * IPv4: 130[.]61[.]64[.]122
    * IPv4: 161[.]97[.]219[.]84
    * IPv4: 130[.]61[.]69[.]123
    * IPv4: 185[.]84[.]81[.]194
    * IPv4: 54[.]36[.]111[.]116
    * IPv4: 192[.]3[.]165[.]37
    * IPv4: 162[.]243[.]19[.]47
    * IPv4: 63[.]231[.]92[.]27
    * IPv4: 80[.]152[.]203[.]134
    * IPv4: 42[.]112[.]26[.]36
* 💡 Security recommendations : Mettez à jour les dispositifs TBK DVR vers les versions corrigées. Effectuez une réinitialisation d'usine si votre appareil est vulnérable et exposé. Évitez d'exposer les dispositifs IoT/DVR sur Internet si ce n'est pas strictement nécessaire.