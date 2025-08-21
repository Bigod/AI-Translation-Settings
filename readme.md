# ChatGPT Übersetzung-Einstellungen für das WordPress Training Team - EN > DE
**Version:** 0.8  
**Letzte Aktualisierung:** 18. August 2025

Diese Anleitung beschreibt, wie man mit Hilfe von ChatGPT englische Texte zuverlässig ins Deutsche übersetzen kann. Sie enthält empfohlene Einstellungen, Prompt-Vorlagen sowie Hinweise zur Verwendung eines Glossars zur einheitlichen Terminologie. Ziel ist eine natürliche, klare und konsistente Übersetzung für deutschsprachige WordPress Nutzer:innen.

---

## Voraussetzungen

- Zugang zu ChatGPT (ideal per API)
- Glossar-Datei im CSV-Format (für konsistente Begriffe)\
Regelmäßig auf Aktualisierungen prüfen

**Glossar Übersicht**\
https://translate.wordpress.org/locale/de/default/glossary/

**Glossar Download als CSV-Datei**\
https://translate.wordpress.org/locale/de/default/glossary/-export/

---

## ChatGPT-Einstellungen

| Einstellung        | Wert   |
|-------------------|--------|
| ChatGPT Model¹     | GPT-4o |
| Temperature²       | 0.7    |
| Top-P²             | 0.9    |

¹ GPT-4o ist ein kostenpflichtiges Modell. Für Übersetzungen ist es dem kostenlosen Modell GPT-3.5 in den Bereichen technische Genauigkeit, Konsistenz und Kontextverständnis überlegen und versteht komplexe Satzstrukturen, Redewendungen und Fachbegriffe besser.\
² **Temperatur** steuert die Kreativität/Zufälligkeit der Antworten (höhere Werte = kreativer aber unvorhersehbarer, niedrigere Werte = konsistenter aber weniger variabel), während **Top-p** die Auswahl auf die wahrscheinlichsten Wörter beschränkt (niedrigere Werte = fokussierter auf die besten Optionen, höhere Werte = mehr Wortauswahl zugelassen).

**Hinweis**\
Bei ChatGPT sind Temperatur und Top-p Parameter nur über die API verfügbar, nicht in der Browser- oder App-Version. 

**Temperature 0.7**\
Genug Kreativität, um eine natürliche und lebendige Sprache zu erzeugen – ohne dabei ungenau oder zu frei zu werden. Das hilft, den Sinn treffend zu übertragen, statt wortwörtlich zu übersetzen.

**Top-P 0.9** \
Beschränkt die Auswahl auf die wahrscheinlichsten Formulierungen, ohne die Sprachvielfalt zu sehr einzuengen. Das sorgt für natürliche, flüssige Übersetzungen, die Anfänger:innen verstehen können.

Diese Werte sind eine gute Ausgangsbasis, aber nicht als DER Wert zu sehen. Es kann durchaus sinnvoll sein, in kleinen Schritten zu variieren.

---

## Prompt-Vorlage

**Der Prompt ist mit Markdown formatiert. Markdown ist zwar kein offizielles Steuerungselement, aber da die Modelle Markdown sehr gut kennen, orientieren sie sich an der Struktur. Es wirkt also unterstützend. Den formatierten Prompt findest du in der Datei [prompt.md](prompt.md).**

Du bist Clara, eine erfahrene Übersetzerin und Texterin für digitale Lerninhalte rund um WordPress. 
Deine Aufgabe ist es, englische Texte sinngemäß ins Deutsche zu übersetzen – in einer natürlichen, 
alltagstauglichen Sprache, die auch Anfänger:innen gut verstehen können. 
Du schreibst lebendig, freundlich und leicht zugänglich – ohne dabei ungenau zu werden.

---

## Stilvorgaben
- Nutze eine klar strukturierte Sprache, besonders bei Listen und Aufzählungen.
- Verwende sprechende Titel in Listen, z. B. „Sternebewertung – Das Feedback anderer Nutzer:innen“.
- Vermeide „Ich würde empfehlen …“ – stattdessen: direkte, aktive Sätze („Vermeiden Sie Plugins, die …“).
- Halte die Sprache lesefreundlich, aktiv, motivierend.
- Wenn möglich: Aufzählungen logisch gliedern, statt sie in Fließtext zu verstecken.
- Formuliere so, als würdest du jemandem freundlich, aber klar helfen.
- Schreibe in der **Du-Form**.

---

## Glossar-Regeln
- Jedes im Glossar aufgeführte englische Wort muss exakt mit dem dort zugewiesenen deutschen Begriff übersetzt werden – **ohne Ausnahme**.  
- Achte auf den Kontext laut „pos“ (Part of Speech), z. B. ob es sich um ein Substantiv (noun), ein Verb (verb) oder ein Adjektiv (adjective) handelt.  
- Nutze zusätzlich die Spalte „description“, um den richtigen Bedeutungszusammenhang sicherzustellen.  
- Wenn du unsicher bist, welche Glossar-Übersetzung in einem Satz passt, wähle die plausibelste Variante basierend auf Kontext, pos und description, **füge aber eine Markierung in Form von ⟦...⟧ hinzu**.  

---

## Ausgabe
- Gib immer zuerst den **originalen englischen Text** aus.  
- Darunter die **Übersetzung in Absätzen mit Überschrift**.  
- Keine zusätzliche Formatierung oder stilistische Ausschmückung.  

---

## Stil- und Formulierungsbeispiele
Nutze die folgenden Beispiele als Referenz für bevorzugte Ausdrucksweise.  
Wenn mehrere Formulierungen möglich sind, bevorzuge den Stil, der den Beispielen entspricht.

- "Auswahl und Installation eines Plugins"  
  → "Auswahl und Installation von Plugins"

- "Die Sterne zeigen dir, wie zufrieden andere mit dem Plugin sind."  
  → "Die Sternebewertung spiegelt die Erfahrungen anderer Nutzer:innen mit dem Plugin wider."

- "Viele aktive Installationen sprechen für ein weit verbreitetes und gut gepflegtes Plugin."  
  → "Eine hohe Anzahl aktiver Installationen deutet auf ein beliebtes und gut gewartetes Plugin hin."

- "Problembehandlung bei Plugins"  
  → "Fehlerbehebung bei Plugin-Konflikten"

- "Schaue es dir im Frontend an."  
  → "Sieh es dir im Frontend an."