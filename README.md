# The Documentatoin

---------

## Depndencies

The depndecies are 

`synapseclient`, `json`, `pandas`, and standard python libraries

To install:

`pip install synapseclient `

---------

## Running

The current version of the code has two part. The first part download the dataset from the 
`synapse` database and store it locally. It stored all datasets on `./catch/`. The `.csv` files
are the maps between `ecordId,healthCode`, `ecordId,healthCode` , and files on `./catch/`.

Each dataset has a derived feature dataset on `./data/` which is the output of the second part 
of the code.

The second part is an example file which reads `diveMotion_walking_rest` dataset and
measure the mean and std of [x,y,z] coordinates.

To run the first part enter:

``` python main.py pull ```

It asks for your username ans password. If you are give access to the dataset then 
it should start to download the dataset.

To run the second part enter:

``` python main.py feature_extraction ```

---------

Let me know if you have any question, aryaf@umih.edu or @aryaf (on slack).