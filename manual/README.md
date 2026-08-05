# Manual results drop box

Add a file named `YYYY-MM-DD.txt` (the puzzle day, Pacific time) with one
line per game, results comma-separated in finish order:

    queens: matt 0:42, kyle 1:03, andrew 1:10
    tango: none          # nobody played
    # comments and blank lines are ignored

Omitted players are DNP; identical scores tie. Games you leave out keep
whatever data the scraper already has. The nightly run on the league PC
picks files up, applies them, and moves them into `processed/`. If a file
has problems, a `.errors` report appears next to it — fix the file and it
retries on the next run.

Easiest way to add a file: https://mflesc0704.github.io/puzzle-league/enter.html
