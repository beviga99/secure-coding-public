# Broken Authentication

- https://www.owasp.org/index.php/Top_10-2017_A2-Broken_Authentication

## Ariketa

Login prozesua egiten duen aplikazio seguru bat diseinatu behar da. Formulario bat izango du erabiltzaileak bere izena eta pasahitza sartzeko. Erabiltzailek kredentzial egokiak baldin baditu, aplikazioaren gune nagusira sartuko da, bestela errore mezu bat eta berriro hasierako formulariora berbideratuko da. Kontutan hartzekoak: HTTP GET/POST, HTTPS, password, hash, session, Two-Factor authentication, Oauth2, ...

begiratu github, google, ... zerbitzuen login prozesuen ezaugarriak.

### Pausoak

1 - Login aplikazio sinple bat egin: Formulario bat. Datu-base batean taula batean erabiltzaileak sartuak ditu. Pasahitzak bere horretan gordetzen dira.

2 - Pasahitzen kontrola. Luzera, asmatzeko zailtasuna ...

3 - Pasahitza Hash bezal gorde. (Bezeroan pasahitzaren hash egin eta bidali? edo zerbitzariak haseatu?)

4 - Session babesa.

5 - MFA-2FA: Two-Factor authentication inplementatu.

6 - Robotak ekiditeko sistema. CAPTCHA

7 - Pasahitza behar ez duten loginak: Oauth, OpenID, ...

8 - Informazioa TSL/SSL HTTPS erabiliz bakarrik. Zertifikatuak.

9 - Pasahitza berreskuratzeko prozesua

10 - Besterik: ...



Puaso bakoitzean aplikazioaren segurtasu arazoak identifikatu eta soluzioak planteatuko dira demo baten bitartez. Garatu dugun aplikazioa "testeatuko" dugu (keyloger, CSRF, XSS, session, brute force, SSL/TLS decryption, session hijacking, ...) eta dituen zuloak identifikatu ondoren soluzioak inplementatuko dira.

Zati bakoitzaren demoa guztiak app batean bilduko dira.

## Erreferentziak

- https://medium.com/@richb_/easy-two-factor-authentication-2fa-with-google-authenticator-php-108388a1ea23
- https://github.com/sonata-project/GoogleAuthenticator

- https://www.sitepoint.com/2fa-in-laravel-with-google-authenticator-get-secure/
