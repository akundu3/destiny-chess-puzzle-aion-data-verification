# AION Archives Automation
## Author: Bungie user - Adi#8888

This script automates interactions with the [AION Archives](https://www.aion-archives.net/) website. It performs the following tasks:

- Opens a connection on the site.
- Inputs a 4-digit frequency using on-screen buttons.
- Pastes a FEN string from the clipboard using the site's Help icon.
- Submits the form.
- Captures the alert or error message from the output console.
- Saves the results into a CSV for analysis.

---


## 🛠 Requirements

- Python 3.7+
- Google Chrome
- ChromeDriver (compatible with your version of Chrome)

### Install Dependencies

```bash
pip install selenium pandas pyperclip
```

## Output Format
frequency,fen,alert_message,success
1849,kBrPQbRq/r6p/P6R/q2nn2B/B2nn2q/R6k/p6r/qPnbKpRr,ALERT: Data Found!,True
2979,nqKRnQkr/p6r/q6N/B2PP2Q/r2PP2k/P6R/K6n/pqNrkQnR,ALERT: Data Found!,True
646,kbKPrBkK/q6K/B6P/R6N/K6b/K6q/b6p/KnBqpNbr,ERROR: Quantum spin Fai0x71=91207,False
61,bqBRpQbR/Q6R/b6R/R2RR2R/p2RR2R/q6R/N6R/PpRBqPrR,ALERT: Data Found!,True
1266,rKRNqkrn/b6p/N6k/p6b/k6N/B6P/n6Q/rkrnQKRp,ALERT: Data Found!,True