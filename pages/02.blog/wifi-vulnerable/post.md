---
title: 'La teva WIFI és vulnerable'
date: '16-10-2017 23:00'
author:
    name: diactoros
    email: diactoros@protonmail.com
---

## Què ha passat

El protocol WIFI WPA2, actualment de major seguretat, és vulnerable a un nou atac informàtic. Qualsevol persona interessada, en un parell de minuts, pot interceptar tota la informació que comparteixes a internet: inclòs contrasenyes a Facebook, Gmail, dades bancàries, tarjetes de crèdit, comunicacions e-mail, etc. Tots els dispositius WIFI són vulnerables, encara que estiguin protegits sota contrasenya.

Publicat oficialment el 16 d'Octubre de 2017 (però filtrat uns dies abans), l'estudiant de post-doctorat Mathy Vanhoef [descriu detalladament la vulnerabilitat del protocl WPA2](https://papers.mathyvanhoef.com/ccs2017.pdf), que teòricament protegeix les comunicacions WIFI amb encriptació asimètrica. Especialment vulnerables són més del 30% de dispositius Linux i Android, inclosos mòbils i tablets.

L'atac consisteix en replicar la xarxa WIFI a la qual un dispositiu es connecta, i alterar el protocol de *4-way handshake*, que gestiona la connexió i pacte entre dispositius, en quant a seguretat es refereix. Així, l'atacant enganya el dispositiu (mòbil, tableta, portàtil...), i aquest accepta una connexió falsificada i no segura. Una vegada la connexió s'estableix, l'atacant pot llegir amb més o menys facilitat tota la informació que el dispositiu transfereix a través d'internet. Fins i tot és vulnerable tota informació transmesa a través de SSL (el cadenat verd que apareix a la barra de navegació del navegador), teòricament no vulnerable a atacs *man-in-the-middle* (*home al mig* de la comunicació), doncs es tracta d'una vulnerabilitat encara més fonamental. Per a entendre la gravetat de la situació: l'atacant no necessita descobrir la contrasenya de la nostra xarxa WIFI.

Tot i que Vanhoef afirma que la *demostració de seguretat* del protocol WPA2 no s'ha contradit, la vulnerabilitat radica en una qüestió tècnica de tota implementació. Això exalta, altre cop, la importància de considerar les demostracions de seguretat matemàtiques com *un factor més* que afirmen la solidesa del protocol, *però no l'únic*.

## Què s'ha de fer

Queda així destruïda la ratxa de 14 anys ininterromputs de seguretat del protocol WPA2. L'expert assegura que la vulnerabilitat obliga a actualitzar el protocol WPA2, tot i que es pot fer de forma compatible amb implementacions antigues. La solució més immediata és simplement **actualitzar els nostres dispositius a la versió més recent**.

La vulnerabilitat es va compartir de forma privada amb companyies d'aparells informàtics a partir del 14 de Juliol de 2017, i les actualitzacions ja estan arribant. Tot i això, res assegura, que agents no-bondadosos tinguessin coneixement de al vulnerabilitat *abans que Vanhoef la descobrís*; caldrà esperar per conèixer l'impacte que ha tingut.

## Bibliografia
- Vanhoef, M. & Piessens, F. *"Key Reinstallation Attacks: Forcing Nonce Reuse in WPA2"* (Octubre 2017).
