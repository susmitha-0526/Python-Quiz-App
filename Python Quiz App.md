# Python Quiz App

Browser version of my Python capstone project. Ten questions on core Python, graded the same way as the command-line app.

## Start a round

Your name

Questions

Result

## Leaderboard

| # | Name | Score | Date |
| --- | --- | --- | --- |

No scores yet. Finish a round to add yours.

## How the Python version works

Questions are validated when loaded from `data/questions.json`. Scores go to `scores.json`. Errors and events are written to `quiz_app.log`.

```
def grade(score, total):
    pct = score / total * 100 if total else 0
    if pct >= 90: return "Excellent"
    if pct >= 70: return "Good"
    if pct >= 50: return "Fair"
    return "Keep practising"
```