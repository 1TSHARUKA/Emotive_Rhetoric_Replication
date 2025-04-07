<h1 align="center"> Playing to the Gallery: Emotive Rhetoric in Parliaments </h1>
<h3 align="center"> A Replication Study </h3>  

<br>

## Project Overview

This repository contains the replication materials for the paper:

OSNABRÜGGE M, HOBOLT SB, RODON T.\
"Playing to the Gallery: Emotive Rhetoric in Parliaments. American Political Science Review."

This project replicates key analyses from the original study, specifically:

1. **Replication of Table 1**: Emotive and neutral speeches example.
2. **Replication of Figure 2**: The development of emotive rhetoric by type of debate from 2001 to 2019.
3. **Replication of Table 3**: Regression analysis of emotive rhetoric
4. **Replication of Figure 4**: Average emotive rhetoric by topic
5. **Extension**:

## Replication summary

### Replication 
In this replication project, we reproduced key empirical results from the original study on emotive rhetoric in parliamentary speeches. First, we replicated Table 1, which presents examples of speeches with high and low levels of emotive rhetoric, illustrating how the scoring system captures variations in tone and sentiment. Second, we recreated Figure 2, which shows the development of emotive rhetoric over time by debate type from 2001 to 2019, confirming trends such as increased emotiveness during high-profile political debates. Third, we replicated Table 3, the regression analysis that quantifies the relationship between debate types and emotive rhetoric scores, finding consistent effect sizes and statistical significance with the original paper. Lastly, we replicated Figure 4, which highlights the average level of emotive rhetoric by topic, reaffirming that certain policy areas, such as social and moral issues, are more emotionally charged than others. Overall, the replication confirms the robustness of the original study’s findings and demonstrates the effectiveness of the emotiveness measure.

### Extension

<!-- Data Availability & Setup -->
<h2 id="data"> Data Availability & Setup</h2>

This replication builds upon the original dataset from the *“Playing to the Gallery”* study. Because of file size limitations on GitHub, the data files cannot be committed directly to this repository. To access the necessary files:

* Please download the original data from the <a href="https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/QDTLYV" target="_blank">
      Harvard Dataverse
    </a>
  as specified by the authors.
* Additionally, all files used in this replication—<code>uk_data</code>, the extended version <code>uk_data_clean</code>, and <code>corpus.txt</code> used for Word2Vec training—are hosted on     <a href="https://drive.google.com/drive/folders/1l8mttWYBo1k-GKExBtYCS9ogwWZ5ZTyF?dmr=1&ec=wgc-drive-hero-goto" target="_blank">
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



<!-- CONTRIBUTORS -->
<h2 id="contributors">Contributors</h2>

<p>
This replication study was conducted as part of the Replication Exercise 2 for 
PPOL 6801 - Text as Data (Spring 2025) at 
<a href="https://mccourt.georgetown.edu/">Georgetown University, McCourt School of Public Policy</a>.
</p>

We thank the original authors for making their data and code publicly available, and Professor Nejla Asimovic for guidance on this replication exercise.

<ul>
  <li><strong>Amber Ni</strong> - <a href="mailto:xn8@georgetown.edu">xn8@georgetown.edu</a></li>
  <li><strong>Tian Tong</strong> - <a href="mailto:yt583@georgetown.edu">yt583@georgetown.edu</a></li>
</ul>

