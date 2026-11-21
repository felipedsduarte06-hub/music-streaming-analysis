# Music Streaming Analysis

Do music playback volumes vary by city and day of the week? This project uses Python and pandas to compare Springfield and Shelbyville across three weekdays. It is a portfolio adaptation of Felipe Duarte's Sprint 2 project in the TripleTen Data Science Bootcamp.

## Results

| Day | Springfield | Shelbyville |
| --- | ---: | ---: |
| Monday | 15,740 | 5,614 |
| Wednesday | 11,056 | 7,003 |
| Friday | 15,945 | 5,895 |

Springfield recorded more playbacks every day and peaked on Friday. Shelbyville peaked on Wednesday, when Springfield recorded its lowest count. These results describe aggregate playback events in the sample. A per-user comparison would require the number of distinct active users in each group.

## Reproduce the analysis

1. Download the [TripleTen dataset](https://practicum-content.s3.us-west-1.amazonaws.com/datasets/music_project_en.csv) and save it as `data/music_project_en.csv` in this project folder. The CSV is hosted by the course provider.
2. From the project folder, install the dependencies with `python -m pip install -r requirements.txt`.
3. Run `jupyter lab`, open [music_streaming_analysis.ipynb](music_streaming_analysis.ipynb), and run all cells.

The notebook standardizes column names, fills missing music metadata, removes 3,826 exact duplicate records, consolidates genre labels, and calculates the six counts above.
