# Melodic Originality in Classical Music

> **[A computational analysis on the relationship between melodic
originality and thematic fame in classical music from the
Romantic period.](https://arxiv.org/abs/2210.12201)**

*Hudson Griffith, griffithh@ufl.edu*

[arXiv:2210.12201](https://arxiv.org/abs/2210.12201)


This is the source code for a computational analysis on the relationship between melodic originality and thematic fame in classical music from the Romantic period. This research was done for the 2021 AP Research performance task and scored a perfect score. The entire research paper and code was created by myself, Hudson Griffith.

## Background

This research was done to propose a novel approach for calculating melodic originality by using every single note in a musical piece. Below is the novel formula.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://i.imgur.com/Ovsfxg0.png" width="400">
  <source media="(prefers-color-scheme: light)" srcset="https://i.imgur.com/ellNfTR.png" width="400">
  <img src="https://i.imgur.com/bckFq29.jpeg">
</picture>

This formula can be applied a to a variety of musical genres. The only required data is a midi file for a specific song. Please refer to the research paper linked above for more information. If you would like to use this code to perform your own analysis on melodic originality please refer to the `Usage` section below.

## Data
To find the data produced for this research please refer to the `data` folder in this repository. There you will find `Final Data.xlsx`, this is a table of every single classical piece tested, its composer, and its calculated melodic originality. A total of 428 pieces were tested. There is also `midi.csv` this file provides information on the piece and composer of a given midi file.

For more detail on the note-transition counts for each piece refer to the `pieces` folder. Here you will find CSV files noting the sum of all two note-transitions for each piece tested.

## Results

The results for this research was that there is no correlation between
melodic originality and thematic fame in the 428 Romantic period
pieces that were analyzed. As seen in the scatter plot below there was no correlation. In the matrix to the left we can see the probability of each two note-transition for all the 428 tested pieces. Please refer to the research paper for more detailed results and conclusions.

![results](https://i.imgur.com/sLc2aqG.png)


## Usage

The source code for this project is in the form of Jupyter Notebooks. Below is an explanation of the individual notebook files and their use cases.

### Matrix Calculation.ipynb
This is the notebook to calculate the two note-transition counts for each piece. Given a `data/midi` folder it will calculate the two note-transition counts and place a file for each piece in `data/pieces`.

### Originality.ipynb
This is the notebook that will calculate and record the melodic originality for a given midi file. You will need a complete `data/pieces` folder with all two note-transition counts for each piece as well as a `data/midi.csv` that is properly formatted.

### Graph.ipynb

This is the notebook that will provide useful graphs and data regarding a complete data set of two note-transition counts. Including heat maps, distribution plots, bigram counts, and more.

### Popularity.ipynb (Optional)

This is the notebook that was used to calculate the thematic fame or popularity of each piece that was tested in the research paper. This is not necessary for calculating melodic originality.


## Contributions/Recommendations
Pull requests are welcome. For any issues or major changes, please open an issue first.

## License
[MIT](https://choosealicense.com/licenses/mit/)
