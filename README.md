# Final Project — Monte Carlo Gacha Game Simulation
Alex Hoang

## Significant Files
- gacha_sim.ipynb — Our jupyter notebook simulation file
- gacha_sim_report.tex - The report LaTeX file that generates the PDF report. Note that generating it may spawn the pdf under "gacha_sim_report.pdf".
- Hoang_Alex_FinalProject.pdf — The actual PDF export from the .tex file.
- outputs/ — Directory holding generated graphs and `results.json` (re-populated on each notebook run).
- Other files may just be a result from compiling the LaTeX file.

## Running the Code
Running the code should be as simple as opening a Jupyter Notebook reader and running it cell-by-cell. Before running, notice the warning above. I set the seed to 42 as that seems to be a common seed used in our in-class labs.

## Recompiling the LaTeX code
I struggled to find a super clean way to recompile the LaTeX code since this was my first full blown LaTeX paper. If you would like to recompile the pdf, the method below is what I used. Do note that you will need a TeX distro and make sure that your pdflatex tool working.

First, navigate to the project root directory in a terminal.
Then, run the following script:
```bash
pdflatex -interaction=nonstopmode gacha_sim_report.tex && pdflatex -interaction=nonstopmode gacha_sim_report.tex
```

-interaction=nonstopmode allows pdflatex to ignore errors and just renders them anyways
