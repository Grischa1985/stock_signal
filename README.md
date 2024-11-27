Aktienanalyse und Deep-Learning-Modell
Projektübersicht

Dieses Projekt kombiniert technische Aktienanalyse und Deep Learning, um mögliche Handelschancen auf Basis historischer Kursdaten zu identifizieren. Es werden Indikatoren wie RSI, Stochastic Oscillator, EMA (Exponential Moving Average) sowie ein neuronales Netzwerk verwendet, um Signale zu generieren und Wahrscheinlichkeiten für Handelschancen zu bewerten.

Funktionen

    Datenbeschaffung
        Lädt historische Aktienkursdaten von Yahoo Finance (yfinance).
        Unterstützt benutzerdefinierte Zeiträume und Intervalle.

    Technische Indikatoren
        Berechnung von:
            Relative Strength Index (RSI) mit talib.RSI.
            Stochastic Oscillator (K- und D-Wert) mit talib.STOCH.
            50- und 200-Tage-EMA mit talib.EMA.

    Signalberechnung
        Handelsindikatoren basieren auf dem Schnittpunkt von EMA50 und EMA200.

    Deep-Learning-Modell
        Ein Keras-Sequential-Modell mit:
            Einem versteckten Layer (Dense mit 1024 Neuronen).
            Einem Ausgabelayer mit sigmoid-Aktivierung zur Berechnung von Wahrscheinlichkeiten.
        Das Modell bewertet Wahrscheinlichkeiten von Handelschancen.
        Modelltraining und Speichern der Gewichte.

    Visualisierung
        Grafische Darstellung der Aktienkursdaten und der berechneten EMAs.
