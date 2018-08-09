# Was ist Keycloak?

Keycloak ist eine Java-basierte Open-Source-Lösung, welche Identitäts- und Zugangs-Management bietet und mit wenigen Zeilen Code in moderne Applicationen eingebunden wird.

Keycloak bietet einet native Benutzerverwaltung, Single Sign-On und die Möglichkeit Social Logins zu nutzen.

Außerdem bietet Keycloak eine hohe Systemsicherheit durch Isolation von der eigentlichen Application. Dadurch dass Keycloak unabhängig von der zu sichernden Application läuft und der Nutzer sich direkt bei Keycloak anmeldet, gewährleistet Keycloak ein hohes Maß an Sicherheit. Durch dieses Vorgehen ist die eigentliche Application von den zu schützenden Benutzerdaten isoliert.

Dadurch werden potenzielle Sicherheitslücken minimiert und ermöglicht Benutzer in verschiedenen Applicationen über eine zentrale Keycloak-Instanz zu authentifizieren.

Nachdem sich der Nutzer bei Keycloak authentifiziert hat wird er zur Application weitergeleitet. Gleichzeitig erhält die Application ein Acces- und ID-Token, welches zur authentifizierung innerhalb der Application dient und zur übertragen Benutzerspeziefischer Daten.

### Nutzerverwaltung

Keycloak bietet verschiedenste Möglichkeiten Nutzer zu authentifizieren bzw. anzulegen. Die einfachste Möglichkeit ist das direkte anlegen/verwalten über die Administrationsoberfläche oder den Nutzern die Möglichkeit einzuräumen sich selbst anzulegen. Desweiteren kann man ein Active Directory oder LDAP-Server einbinden, um gegen dieses zu authentifizieren.  Dabei kann man bestimmte Nutzerdaten beim ersten Login oder manuell in die mitgelieferte Datenbank von Keycloak synchronisieren und somit den nächsten Login beschleunigen. Es ist zu beachten, dass hierbei keine Passwörter gespeichert werden! Zudem ist der Einsatz von Keycloak als Identity Broker möglich, der die Authentifizietung an einen externen Identity Provider oder ein soziales Netz z.B. Facebook oder Github deligiert.

### Singel-Sign On

Nachdem der Nutzer nun eingeloggt ist, kann er alle Applicationen nutzen die ihn zu Keycloak deligiert hätten. Das hat wiederum dan Vorteil, dass Nutzer sich für weitere Services nicht erneut einloggen müssen. Hierbei ist zu erwähnen, nicht alle Nutzer können die selben Bereiche einer Application nutzen. Verschiedene Bereiche einer Application sind mit verschiedenen Berechtigungen verknüpft, welche beim ersten Login bei Keycloak vergeben werden oder händisch gegeben werden. Dadurch wird der Application eine weitere Aufgabe abgenommen und weiter abgesichert.

Zum Thema Rechte und Rollen siehe *hier link einfügen*.

### Administration

