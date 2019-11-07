# DATA 512 FINAL PROJECT 

## Goal for this project:
I'm hoping to look at musician information data to see if there is a relation between genre type/ genre count and view count, to see what kind(s) of genre(s) are more popular as of 6 months ago.

## Link to Dataset:

The dataset is an opensource kaggle dataset found at: https://www.kaggle.com/pieca111/music-artists-popularity

## License for Dataset:

Interestingly although this is an open source dataset, the license is listed as "unknown" : https://www.kaggle.com/pieca111/music-artists-popularity/metadata

## Possible Biases for the data:

- The data has contains viewcounts from a limited source, guaging the "popularity" of an artist may not be possible considering certain people do not even have access to this particular streaming site.

- The data is also only limited to bands listed on the site "musicbrainz" which may not include certain independent artists that may have a niche but strong following.

- Also, streaming counts may not be a great guage of popularity, it may imply a certain song by the band is popular, but not that the band itself is popular (case in point one hit wonders like vanilla ice)

- The recorded genres (artist tags) are also recorded by fans or music listeners, which may not be accurate or reflect what the band itself considers their branding to be.

- The fact that there are so many tags for each artist implies that there will be massive overlap in many genres that should not generally overlap, I may deal with this bias by creating my own major genres and categorizing each artist based on the number of tags of each category the band has and figuring out the majority
