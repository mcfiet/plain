# Textvereinfachung mit Deep Learning - plAIn

Dieses Projekt wurde im Rahmen des Moduls **Advanced Deep Learning** im Masterstudium entwickelt. Ziel ist es, ein neuronales Netz mit PyTorch zu erstellen, das Fließtext automatisch in Leichte Sprache übersetzt.

## Projektidee

**Ziel:** Entwicklung eines Sequence-to-Sequence-Modells, das komplexe deutsche Texte automatisch in Leichte Sprache übersetzt.

## Datenquellen

* [LaMarr-Institut: Datensatz Leichte Sprache](https://lamarr-institute.org/de/blog/datensatz-leichte-sprache)
* [Aktion Mensch](https://www.aktion-mensch.de/)
* [Bundesregierung: Leichte Sprache](https://www.bundesregierung.de/breg-de/aktuelles/faq-leichte-sprache-2189214)
* [Bundesfachstelle Barrierefreiheit](https://www.bundesfachstelle-barrierefreiheit.de/DE/Home/home_node.html)
* [BMAS](https://www.bmas.de/DE/Startseite/start.html)

Zusätzlich wurden eigene Beispieldatensätze händisch erstellt.

## Modellarchitektur

* **Encoder-Decoder Architektur** (Sequence-to-Sequence)
* **Encoder:** BiLSTM
* **Decoder:** LSTM mit Attention-Mechanismus
* **Tokenisierung:** SentencePiece oder Subword-Tokenizer
* **Loss-Funktion:** CrossEntropyLoss
* **Optimizer:** Adam

## Evaluation

* BLEU-Score
* BERTScore
* Qualitative Bewertung durch Textbeispiele

## Projektstruktur - beispielhaft

```
plain/
|
├── notebooks/
|   ├── 01_data_preparation.ipynb
|   ├── 02_model_training.ipynb
|   └── 03_evaluation.ipynb
|
├── data/
|   ├── raw/
|   └── processed/
|
├── models/
|
├── utils/
|   ├── tokenizer.py
|   └── dataset.py
|
├── requirements.txt
└── README.md
```

## Zeitplan (8 Wochen)

| Woche | Aufgabe                                            |
| ----- | -------------------------------------------------- |
| 1     | Projektstruktur, Datenquellen, händische Paare     |
| 2     | Daten sammeln, Tokenizer und DataLoader einrichten |
| 3     | Encoder & Decoder mit PyTorch umsetzen             |
| 4     | Attention-Modul einbauen, Trainingsloop            |
| 5     | Training, Debugging, Logging                       |
| 6     | Evaluation mit BLEU/BERTScore                      |
| 7     | Optional: GUI/CLI, Demo, Berichtentwurf            |
| 8     | Abschlusspräsentation und Bericht finalisieren     |

## Risiken

* Begrenzte Datenverfügbarkeit
* Leichte Sprache ist nicht nur formal, sondern auch inhaltlich/sozial
* Zeitliche Einschätzung schwierig als Erstprojekt im Deep Learning

## Lizenz

Dieses Projekt dient ausschließlich akademischen Zwecken.

---

