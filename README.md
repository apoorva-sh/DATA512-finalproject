# DATA 512 FINAL PROJECT 

## Goal for this project:
To look at the relationship between music and various emotions (as an initial response) By performing basic Exploratory Analysis on [two datasets](#data-description), And answer four main research questions:

#### -  How linear is the relationship between "Melody" and "Mean Emotional Response"?

    Since the melody is already classified in the same buckets as Mean Emotional Response, it would be interesting to know if the overreaching melody type has a predominant affect on the mean emotional response

#### - Which factor most affects the relationship between "Melody" and "Mean Emotional Response"?

    Which of the six musical factors most changes the mean emotional response from co-inciding with the Melody

#### - Does a "minor" mode mostly illicit a "Scary" emotional response?

    As a listener of music generally songs in a minor key can come off as creepy, I would like to know if that holds true for the populous

#### - Does a high tempo leady to a happier emotional response?

    Generally speaking fast tempo-ed songs (such as pop music) geenrate a positive response, it would be interesting to know if that is true here as well

## Link to Original Dataset:

The dataset is available at: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/IFOBRN

## Data Description

The data is hosted on this git repo at: https://github.com/apoorva-sh/DATA512-finalproject/tree/master/Data

### [Design Matrix Table](https://github.com/apoorva-sh/DATA512-finalproject/blob/master/Data/design_matrix.csv)

The design matric table contains information on each stimulus wave. The dataset contains a total of 200 stimuli waves ([link to stimuli](https://dataverse.harvard.edu/file.xhtml?persistentId=doi:10.7910/DVN/IFOBRN/J2D0BN&version=1.0)), these 200 stimuli waves were created by altering an initial sound wave iteratively and factorially by the following 7 properties 

- **Register** - 6 levels
    - 1: 53 MIDI pitch
    - 2: 59 MIDI pitch
    - 3: 65 MIDI pitch
    - 4: 71 MIDI pitch
    - 5: 77 MIDI pitch
    - 6: 83 MIDI pitch
- **Mode** - 2 modes
    - 1: Major key
    - 2: Minor key
- **Tempo** - 5 tempos (in NPS)
    - 1: 1.2
    - 2: 2
    - 3: 2.8
    - 4: 4.4
    - 5: 6
- **Sound level** - 5 sound levels (in dB)
    - 1: -10
    - 2: -5
    - 3: 0
    - 4: +5
    - 5: +10
- **Articulation** - 4 levels (from legato to staccato)
- **Timbre** - 3 levels 
    - 1: trumpet
    - 2: flute
    - 3: horn
- **Melody** - 4 types
    - 1: Sad
    - 2: Scary
    - 3: Happy
    - 4: Peaceful

(It must be noted that the subset of 200 stimuli as opposed to a complete factorial was done by the researchers to focus their research on just the first-interaction level of the above variables. It would have been nice to have a complete set of the factorials so I could ask different or more in-depth questions, but this dataset provides enough information for the scope of this research)

The Melody is categorized as "Sad, Happy, Scary, or Peaceful" based on research conducted previosuly ([Vieillard et al., 2008.](https://www.tandfonline.com/doi/full/10.1080/02699930701503567) The musical excerpts can be used for research with ackowledgements of the copyright, © Bernard Bouchard, 1998.). This study conducted research into the specificties of emotions provoked by the 4 sound waves on their own.

The seven alterable factors were decided based on researcg by [Bresin, R. & Friberg, A. (2011). Emotion rendering in music: range and characteristic values of seven musical variables. Cortex, 47(9), 1068-1081](https://www.ncbi.nlm.nih.gov/pubmed/21696717)

The table contains 8 columns and 200 tuples, each row co-inciding with one stimuli wave.

The columns are : Nro (Stimuli Number), and the 7 characteristics with their respective level:

| Nro | Register | Mode | Tempo | Soundlevel | Articulation | Timbre | Melody |
|-----|----------|------|-------|------------|--------------|--------|--------|
| 1   | 4        | 1    | 4     | 4          | 2            | 2      | 4      |
| 2   | 5        | 1    | 4     | 1          | 1            | 2      | 2      |
| 3   | 2        | 2    | 5     | 1          | 1            | 2      | 1      |

### [Mean Emotional Response Table](https://github.com/apoorva-sh/DATA512-finalproject/blob/master/Data/mean_emotion_ratings.csv)

This table contains the mean responses categorized into 4 major buckets "Scary, Happy, Sad, and Peaceful" for each of the 200 stimuli.

As per the [paper published](https://www.frontiersin.org/articles/10.3389/fpsyg.2013.00487/full) with research on this data, 46 listeners were asked to record their emotional response to each sound stimuli, for each emotional category on a scale of 1 to 7. Thus each listener recorded 4 paralell ratings for each sound stimuli.

These 46 listeners were spread out across two research labs, one in stockholm the other in Jyväskylä.

Thus table contains 5 columns and 200 tuples, with each row corresponding to one sound stimuli.

The columns are: Nro (Stimuli number), and mean score out of 7 for each bucket: scary, Happy, Sad and Peaceful.

| Nro | Scary  | Happy  | Sad    | Peaceful |
|-----|--------|--------|--------|----------|
| 1   | 1.2889 | 4.4667 | 1.7111 | 3.1333   |
| 2   | 1.0667 | 5.4444 | 1.4889 | 4.4889   |
| 3   | 2.0222 | 1.4889 | 3.7778 | 2.7111   |


## License for Dataset:

The license is listed as [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/) as listed in the "Terms" section of the data description

## [License for project:](https://github.com/apoorva-sh/DATA512-finalproject/blob/master/LICENSE)

This project is Under [MIT license](https://opensource.org/licenses/MIT)
