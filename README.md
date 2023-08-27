# Desafio-Intelie-SSH-Parte-2
<br>

![image](https://github.com/andregomesrocha/Desafio-Intelie-SSH-Parte-2/assets/84783787/e11eff65-dc00-47f0-9f08-8a9c286392f4)
<br>
<br>
<b>live.properties</b>
<br>

![image](https://github.com/andregomesrocha/Desafio-Intelie-SSH-Parte-2/assets/84783787/ed7ed118-1c5b-4643-9b59-7eb01acb2634)

<b>pre-run</b>
<br>

![image](https://github.com/andregomesrocha/Desafio-Intelie-SSH-Parte-2/assets/84783787/ea93b5b5-421b-4e7a-b631-754ac0fa90b9)

<b>log compacted from LIVE</b>
<br>

![image](https://github.com/andregomesrocha/Desafio-Intelie-SSH-Parte-2/assets/84783787/a679f53d-3207-4cb4-a183-c0f7d96141ae)

<b>Checking if cron is active</b>
<br>

![image](https://github.com/andregomesrocha/Desafio-Intelie-SSH-Parte-2/assets/84783787/b303632e-ee95-4055-8fe7-eb3a679b80be)

<b>Checking scheduling of the cron</b>
<br>

![image](https://github.com/andregomesrocha/Desafio-Intelie-SSH-Parte-2/assets/84783787/c6badb67-1ad9-46d3-861b-edaf74094503)

<b>Enter with Sudo Su = Root</b>
<br>

![image](https://github.com/andregomesrocha/Desafio-Intelie-SSH-Parte-2/assets/84783787/54d79859-98ab-4025-ad3a-84856208bd72)


<b>Set automatic rotation of application logs (LiVE), where logs older than the current day should be compressed and logs removed with a date greater than 7 days.</b>
<br>

![image](https://github.com/andregomesrocha/Desafio-Intelie-SSH-Parte-2/assets/84783787/5db79d6d-8984-46fb-985f-f8bd8d07131a)

<b>Commands Used to get here:</b>

55 16 * * * find /opt/intelie/live/logs -type f -name "live-*.log" -mtime +7 -exec gzip {} \;

