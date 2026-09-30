Primer, creem l'script que executarem amb el target.
<img width="761" height="95" alt="image" src="https://github.com/user-attachments/assets/45b22f17-eb33-47c2-919d-49db3c9680d0" />

I crem l'script, que en aquest cas, genera una carpeta oculta a "/", i copia les claus d'encriptació dintre d'aquesta.
<img width="789" height="192" alt="image" src="https://github.com/user-attachments/assets/ceb859f0-91f9-4c4c-a2e3-5c4f952bff0e" />

Ara, creem un servei amb sudo nano /etc/systemd/system/nouservei.service
<img width="761" height="95" alt="image" src="https://github.com/user-attachments/assets/48d19828-2c07-4aeb-b487-62d21cbd2d39" />

I posem el text.
<img width="789" height="288" alt="image" src="https://github.com/user-attachments/assets/af783db8-a4ee-456b-a165-d8b1d216c1eb" />


Tot seguit, creem el target amb **sudo nano /etc/systemd/system/script.target**
<img width="761" height="117" alt="image" src="https://github.com/user-attachments/assets/e8a66e12-5c58-4121-aeb4-618964677f88" />

I posem el contingut.
<img width="761" height="168" alt="image" src="https://github.com/user-attachments/assets/ad3a3c69-6700-4b2a-8cec-947ee615f0f7" />

A continuació, farem que sigui default target.

Primer, comprovarem quin és el default target amb **systemctl get-default**

I ho canviarem al script que hem creat.
<img width="761" height="203" alt="image" src="https://github.com/user-attachments/assets/da05dd15-4b1e-4546-81b4-01564962b154" />
