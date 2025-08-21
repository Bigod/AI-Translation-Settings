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