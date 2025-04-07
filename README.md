<h1 align="center"> Playing to the Gallery: Emotive Rhetoric in Parliaments </h1>
<h3 align="center"> A Replication Study with a Dictionary-Based Extension </h3>  


<!-- Project Introduction -->
<h2 id="data"> Overview</h2>

This repository contains a partial replication and dictionary-based extension of the article:
Osnabrügge, M., Hobolt, S. B., & Rodon, T. (2021), Playing to the Gallery: Emotive Rhetoric in Parliaments, *American Political Science Review*, 115(3), 885–899. 
- The official publication can be found online at American Political Science Review:
<a href="https://www.cambridge.org/core/journals/american-political-science-review/article/playing-to-the-gallery-emotive-rhetoric-in-parliaments/2A47C797136261391DA27F3A16F64886
">
      Original Paper
    </a>
- The replication materials are provided within the Harvard Dataverse Network, with direct access: <a href="https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/QDTLYV" target="_blank">
      Harvard Dataverse
    </a>


The original paper examines how legislators strategically use emotive rhetoric in parliamentary speeches—particularly during high-profile debate settings such as Prime Minister's Questions (PMQs) and Queen’s Speech Debates. Using a dictionary-based approach, the authors construct emotion-labeled word embeddings trained on parliamentary corpora, starting from seed words drawn from the Affective Norms for English Words (ANEW) lexicon. Speeches are then scored by their emotive tone, and key hypotheses are tested through a combination of visualizations and regression analyses.

<br>


<!-- Project Replication -->
<h2 id="data"> Replication Summary</h2>

This replication reproduces key empirical results, including:
- `Table 2`: Illustrative examples of emotive and neutral speeches using the original scoring approach
- `Figure 2`: Temporal trends in emotive rhetoric by debate type (2001–2019), highlighting rhetorical peaks during high-profile debates
- `Table 3`: Regression analyses linking institutional settings to variation in emotive tone
- `Figure 4`: Topic-level differences in average emotive rhetoric across policy domains with greater intensity in socially and morally charged domains

These results reinforce the study’s conclusion that emotive rhetoric is deployed strategically in parliamentary settings.


In our **extension**, we construct a new emotive dictionary using the the NRC Emotion Lexicon developed by Saif Mohammad( <a href= "https://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm"> NRC Association Lexicon Link </a>), applying the same Word2Vec-based embedding method to the UK parliamentary corpus. We then compare the outputs and regression results of the original and extended dictionaries across all key components.

Our findings show that dictionary choice significantly affects analytical outcomes—highlighting, for instance, higher emotive intensity in "Urgent Questions" and shifting topic-level rankings (e.g., elevated scores for “Freedom and Democracy”). These differences underscore how lexicon design influences interpretations of emotional language in political discourse. 
> More detailed comparisons, interpretations, and visualizations can be found in the accompanying project report.

<br>

<!-- Data Availability & Setup -->
<h2 id="data"> Data Availability & Setup</h2>

This replication builds upon the original dataset from the *“Playing to the Gallery”* study. Because of file size limitations on GitHub, the data files cannot be committed directly to this repository. To access the necessary files:

* Please download the original data from the <a href="https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/QDTLYV" target="_blank">
      Harvard Dataverse
    </a>
  as specified by the authors.
* Additionally, all large corpus files used in this replication—<code>uk_data</code>, the cleaned and extended version <code>uk_data_clean</code>, and <code>corpus.txt</code> used for Word2Vec training—are hosted on     <a href="https://drive.google.com/drive/folders/1l8mttWYBo1k-GKExBtYCS9ogwWZ5ZTyF?dmr=1&ec=wgc-drive-hero-goto" target="_blank">
      Google Drive
    </a>
 for convenience. These include preprocessed text, learned embeddings, and model outputs.

> **Note:** The `uk_data_clean` file is the extended version of the original dataset that includes additional variables engineered during replication—such as tokenized speeches, cleaned text, emotion scores, and model predictions. Its larger size reflects these enhancements in vocabulary captured for training.

<br>

<!-- PREREQUISITES -->
<h2 id="prerequisites">Prerequisites</h2>

This project is written in the R programming language and requires the following packages:<br>
`tidyverse`, `dplyr`, `readr`, `tidyr`, `stringr`, `tidytext`, `tokenizers`, `ggplot2`, `gridExtra`,`scales`, `lubridate`, `quanteda`, `quanteda.sentiment`, `data.table`, `text2vec`, `wordVectors`

These can be installed using `install.packages()` or loaded via preferred package manager. Additional dependencies may be required for replicating the original paper’s Word2Vec embedding or advanced modeling.


<br>

<!-- Repository Structure -->
<h2 id="project-files">Repository Structure</h2>

<p>
This repository contains datasets, scripts, and output files for our replication study. 
Our replication includes modifications and additional analysis, detailed below.
</p>

---

<h3> Data</h3>

<ul>
  <li><code>emotive_expanded.csv</code> -  Expanded emotive word list derived from the NRC Emotion Lexicon and Word2Vec model </li>
  <li><code>neutral_expanded.csv</code> - Expanded neutral word list using NRC-based seed words and embeddings </li>
  <li><code>emotive_uk.csv</code> - Original paper's emotive word list derived from ANEW-based seeds and trained Word2Vec embeddings on UK parliamentary corpus, which has been provided and utlized in our replication </li>
  <li><code>neutral_uk.csv</code> - Original paper's neutral word list trained using the same method above </li>
</ul>

---

<h3> Scripts</h3>

<ul>
  <li><code>Replication.rmd</code> - Main analysis script that replicates the key figures and tables from the original paper and implements the dictionary-based extension using the NRC lexicon. This file contains code for preprocessing, modeling, scoring, and visualization. </li>
</ul>

---

<h3> Outputs</h3>
All tables and figures generated during this replication are saved in the <code>output</code> directory.  For comparison purposes, the corresponding original versions from the published article are also included and clearly labeled in the file names (e.g., original_dictionary and extended_dictionary etc.).

The final presentation slides and written report are available in the <code>doc</code> folder.


</ul>


<!-- CONTRIBUTORS -->
<h2 id="contributors">Contributors</h2>

<p>
This replication study was completed as part of the Replication Exercise 2 for 
the course PPOL 6801 - Text as Data (Spring 2025) at 
<a href="https://mccourt.georgetown.edu/">Georgetown University, McCourt School of Public Policy</a>.
</p>

We gratefully acknowledge the original authors for publicly sharing their data and code, which made this replication possible. We also appreciate Professor Nejla Asimovic for her invaluable guidance and support throughout the project.

<ul>
  <li><strong>Amber Ni</strong> - <a href="mailto:xn8@georgetown.edu">xn8@georgetown.edu</a></li>
  <li><strong>Tian Tong</strong> - <a href="mailto:yt583@georgetown.edu">yt583@georgetown.edu</a></li>
</ul>

