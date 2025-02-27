1. **Lokale API-Entwicklung:**  
   - Entwickle eine RESTful API, die grundlegende CRUD-Operationen (Erstellen, Auslesen, Aktualisieren, Löschen) für Todo-Einträge ermöglicht.  
   - Setze die API zunächst lokal (localhost) auf, sodass sie über definierte Endpunkte erreichbar ist.

2. **Postman-Umgebung einrichten:**  
   - Konfiguriere ein Postman-Environment für die Entwicklungsphase.  
   - Definiere Variablen (z. B. Basis-URL), die es erlauben, zwischen der lokalen und später der produktiven Umgebung zu wechseln, ohne die Requests selbst anpassen zu müssen.

3. **Testen der API:**  
   - Implementiere in Postman Tests, um die Funktionalität und die korrekte Antwort der API-Endpunkte zu validieren.  
   - Nutze dabei die definierten Environment-Variablen, um flexibel zwischen Umgebungen zu wechseln.

4. **Deployment auf eine Azure-VM:**  
   - Lade die Anwendung nach erfolgreichem lokalen Test auf eine Azure Virtual Machine hoch.  
   - Sorge dafür, dass alle notwendigen Konfigurationsschritte (wie z. B. Firewall-Regeln und Portfreigaben) durchgeführt werden.

5. **Einrichtung von NGINX:**  
   - Installiere und konfiguriere NGINX auf der Azure-VM als Reverse-Proxy, um Anfragen an die API weiterzuleiten.  
   - Achte darauf, dass die Konfiguration den Zugriff auf die API über eine öffentliche URL ermöglicht.

6. **Anpassung der Postman-Umgebung für die Produktionsphase:**  
   - Aktualisiere das Postman-Environment, indem du die URL der Azure-VM (bzw. den über NGINX erreichbaren Endpunkt) als Environment-Variable setzt.  
   - Führe erneut die Tests in Postman durch, um sicherzustellen, dass die API in der produktiven Umgebung korrekt funktioniert.

7. **Dokumentation der Todo-App in Postman:**  
   - Erstelle eine umfassende Dokumentation für die Todo-App innerhalb von Postman.  
   - Dokumentiere die API-Endpunkte, beschreibe deren Funktion, erwartete Parameter, Rückgabeformate sowie beispielhafte Anfragen und Antworten.  
   - Nutze dabei die integrierten Funktionen von Postman zur Erstellung und Verwaltung von Dokumentationen, um einen nahtlosen Informationsfluss zwischen Entwicklung und Endnutzern sicherzustellen.
