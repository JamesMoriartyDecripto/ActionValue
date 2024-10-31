# Calcolatore del valore di un'azione

Un calcolatore interattivo che implementa una formula matematica per valutare oggettivamente quanto vale la pena intraprendere un'azione specifica. Il progetto combina teoria della decisione, matematica e psicologia per fornire un framework quantitativo per il decision-making.

## 📚 Descrizione

Il progetto implementa una formula matematica che considera molteplici fattori per calcolare un "punteggio di valore" per qualsiasi azione o decisione. La formula bilancia benefici, costi e rischi, normalizzando tutti i valori in un intervallo [0,1] per una valutazione coerente.

### Formula base
```math
V_{azione} = \frac{B \cdot P \cdot I}{T + E + S} \cdot (1 + O) \cdot (1 + C) \cdot (1 - R)
```

### Variabili
- **B**: Benefici attesi [0,1]
- **P**: Probabilità di successo [0,1]
- **I**: Impatto a lungo termine [0,1]
- **T**: Tempo richiesto normalizzato (ore/24) [0,1]
- **E**: Energia richiesta [0,1]
- **S**: Stress generato [0,1]
- **O**: Opportunità create [0,1]
- **C**: Coerenza con valori personali [0,1]
- **R**: Rischi potenziali [0,1]

## 🚀 Come iniziare

1. Clona il repository
```bash
git clone https://github.com/username/value-calculator.git
```

2. Apri `ActionValue.html` nel tuo browser
3. Usa gli slider per inserire i valori
4. Ottieni immediatamente il risultato calcolato

## 💻 Tecnologie utilizzate

- HTML5
- CSS3
- JavaScript (Vanilla)
- MathJax per il rendering delle formule matematiche

## 📖 Come usare

1. **Valutazione delle Variabili**
   - Considera ogni variabile attentamente
   - Usa i slider per impostare valori tra 0 e 1
   - Il tempo viene automaticamente normalizzato su 24 ore

2. **Interpretazione dei risultati**
```
v > 0.8         → Altamente consigliato
0.5 < v ≤ 0.8   → Vale probabilmente la pena
0.3 < v ≤ 0.5   → Da valutare attentamente
v ≤ 0.3         → Probabilmente non vale la pena
```

## ⚠️ Limitazioni

- La formula assume indipendenza tra le variabili
- Non considera fattori puramente emotivi
- Il peso delle variabili è uniforme
- Non tiene conto di interdipendenze complesse

## 🔧 Personalizzazione

È possibile modificare:
- Range degli slider
- Pesi delle variabili
- Soglie di interpretazione
- Stile dell'interfaccia

## 🤝 Come contribuire

1. Fork del repository
2. Crea un branch per le modifiche
```bash
git checkout -b feature/nuova-feature
```
3. Commit e push delle modifiche
4. Apri una Pull Request

## 📋 TODO

- [ ] Aggiungere salvataggio configurazioni
- [ ] Implementare export/import dei dati

## 🙏 Riconoscimenti

- Ispirato dalle teorie della decisione razionale
- Framework matematico basato su principi di analisi costi-benefici
- Design influenzato da best practice UX/UI moderne

---

*Nota: Questo progetto è uno strumento di supporto decisionale, non un sostituto del giudizio personale.*
