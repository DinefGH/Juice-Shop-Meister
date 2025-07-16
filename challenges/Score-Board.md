### Miscellaneous

# Score Board ★

Find the carefully hidden 'Score Board' page.
<br />


### Vulnerability Impact

Verschiedene Schwachstellen umfassen ein breites Spektrum von Fehlern - wie Fehlkonfigurationen, unsichere Standardeinstellungen und Fehler in der Geschäftslogik -, die Angreifer ausnutzen können, um Kontrollen zu umgehen, Daten zu verlieren oder Dienste zu stören.<br />



![Score Board Path](/img/score-board-path.png)
<br />

![Score Board](/img/score-board.png)

<br />
#### Prerequisites

- OWASP Juice Shop running at `http://127.0.0.1:3000/#/`
<br />

#### Steps to Reproduce
<br />

1. **Open OWASP Juice Shop** 
- Navigate to `http://127.0.0.1:3000/#/`.
<br />


2. **Open Dev Tools**
- Right‑click on the page and choose **Inspect**, or press `F12`.  
<br />


3. **Go to the Sources panel**  
-  In DevTools, select **Sources** and locate the `main.js` file.
<br />


4. **Search for `score-board`**  
- Press `Ctrl+F` and enter `score-board`.  
- The 7th occurrence shows the hidden route for the Score Board.
<br />  


5.  **Check for the Scorboard** 
- Copy the discovered path (e.g. `score-board`) into your browser’s URL bar
<br />


> **Tip:** While browsing `main.js`, look for other route names (e.g. `administration`)—they often point to additional hidden pages or challenges.
