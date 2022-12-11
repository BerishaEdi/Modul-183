# Lern-Bericht M183 Cross-Site-Scripting
Eduard Berisha

## Einleitung

In diesem Lernbericht möchte ich auf Cross-Site-Scripting (XSS) eingehen. Cross-Site-Scripting ist eine Art von Cyberangriff, bei dem bösartiger Code auf einer Webseite eingeschleust wird, um die Interaktion von Benutzern mit der Webseite zu manipulieren. Dies geschieht, indem der Angreifer versucht ein Script als Eingaben in einem Formularfeld auf der Webseite einzuschleusen.

## Was habe ich gelernt?

Ich habe gelernt das ich eingaben von Benutzern filtern muss und alle Zeichen umschreiben soll die für einen XSS-Angriff genutzt werden könnten.

## Beschreibung

✍️ Verwenden Sie drei verschiedene Medien, um zu zeigen, was Sie gelernt haben. Zum Beispiel:
```Java
// Filtert die Eingabe und ersetzt verdächtige Zeichen
public String bereinigeInput(String userInput) {
  return userInput.replaceAll("<", "&lt;").replaceAll(">", "&gt;");
}

// Beispiel für die Verwendung des Filters
String userInput = "<script>alert('XSS')</script>";
String bereinigeInput = sanitizeInput(userInput);
```
In diesem Beispiel wird eine Methode bereinigeInput() definiert, die die Benutzereingabe filtert und alle Zeichen entfernt, die für einen XSS-Angriff genutzt werden könnten. Die Methode wird dann verwendet, um die Benutzereingabe zu filtern und bösartigen Code zu entfernen.
![ezgif com-gif-maker](https://user-images.githubusercontent.com/69904270/206932366-7ab603e5-142c-4b1e-88ca-12676ea05b05.gif)
Wie man sehen kann wird das Script nicht ausgeführt da er ausgefiltert wird.


## Verifikation

Der Code ausschnitt und die Beschreibung zeigen, wie ich die IT-Gefahr vermeiden kann. Im Code abschnitt sieht man das ich die wichtigsten Zeichen für die Einschleusung unerwünschten Codes richtig gefiltert und entschärft habe und im GIF sieht man das es erfolgreich funktioniert hat.

# Reflektion zum Arbeitsprozess

👍 Ich habe das Prinzip von XSS schnell und gut verstanden und mir war schnell bewusst welche Massnahmen ich ziehen muss um solche Angriffe zuvorzukommen.

👎 Die Umsetzung lief im Grossen und Ganzen nicht schlecht jedoch musste ich zuerst im Internet und in den Schuldokumenten einige Informationen sammeln, um es dann sicher anwenden zu können.

In der Zukunft möchte ich mich von Anfang an auf etwas fokussieren bis ich es nahezu mühelos anwenden kann um so unötige zeitvherschwendungen zu vermeiden.
