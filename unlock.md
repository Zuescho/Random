# Aachener Zeitung Unlock

## Update 14.04.2023 broken...  

Die Aachner Zeitung setzt jetzt auf Cloudflare und blockt sobald man sich al googlebot meldet, wahrscheinlich sind nur einzelne IP ranges jetzt freigeschaltet.  
Daher das ganze funktioniert hier nicht mehr...  
Als Alternative kann man sich das noch über https://search.google.com/test/rich-results/result?id=MYy1AOPpMGDxY6NukhcbNw holen.  
Oben in der Zeile die URL vom Artikel rein und dann auf `Getestete Seite Anzeigen` klicken, dort dann wiederum auf `Screenshot`.

>Aachner Zeitung lesen ohne Abo? Kein Problem!

Vorraussetzungen:

- Firefox (Chrome, Android auch möglich beschränke mich hier aber auf FF)
- https://addons.mozilla.org/de/firefox/addon/bypass-paywalls-clean/

Nach der Installation muss man für die Aachener Zeitung noch eine eigene Regel erstellen.

![](attachments/aachen_unlock_001.png)


![](attachments/aachen_unlock_002.png)

Unten im Bereich Json file, dann folgende Regel hinzufügen und speichern.
````
{"Aachen":{"domain":"aachener-zeitung.de","block_javascript":1,"block_javascript_ext":1,"useragent":"googlebot","random_ip":"eu"}}
````

**Fertig**

Jetzt kann man schon das ganze Angebot ohne Abo nutzen.  
Falls es zu Problemen mit der Darstellung kommt, ruhig mal die Seite mit F5 neuladen und darauf achten das hier oben das Addon eingeschaltet ist.

![](attachments/aachen_unlock_003.png)

![](attachments/aachen_unlock_004.png)
