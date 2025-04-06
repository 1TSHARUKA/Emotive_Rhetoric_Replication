<h1 align="center"> Playing to the Gallery: Emotive Rhetoric in Parliaments </h1>
<h3 align="center"> A Replication Study </h3>  

<br>

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

