# PykaDex Docs.
## Welcome to PykaDex Docs

Gotta classify them all.

# repos explained
For time being as docs are being worked on.  This is a quick run down of the pykadex repositories and their uses.

## [PykaDex_Trainer](https://github.com/PykaDex/PykaDex_Trainer)
- main repo for creating and training nueral nets models to classify pokemon. using the data generated/augmented by PykaDex_Data. Plan to train using azure are being discussed

## [PykaDex_Data](https://github.com/PykaDex/PykaDex_Data/)
- repo for data augmentation and formating ready to feed into Pykadex_Trainer

## [PykaDex_WTP (whos that pokemon)](https://github.com/PykaDex/PykaDex_WTP/)
- repo for test a model by suppy an image of a pokemon and then predicting

## [PykaDex_API](https://github.com/PykaDex/PykaDex_API/)
- repo for api/web based utilisatin of Pykadex_WTP

## [PykaDex_DSi](https://github.com/PykaDex/PykaDex_DSi/)
- repo for dsi homebrew with the end goal of turn a nintendo dsi into a functional pokedex by using Pykadex_API

## [PykaDex_Mobile](https://github.com/PykaDex/PykaDex_Mobile/)
- repo for dsi homebrew with the end goal of turn android phone into a functional pokedex by using Pykadex_API

## [PykaDex_Docs](https://github.com/PykaDex/PykaDex_Docs/)
- repo for documentation across all things pykadex related (currently using github pages as host)

## [PykaDex_Old](https://github.com/PykaDex/PykaDex_Old/)
- archived repo of old project that used tensorflow orginally

## [PykaDex_Clembot](https://github.com/PykaDex/PykaDex_Clembot/)
- repo for a discord bot with the end goal of being able to use Pykadex_api though discord chats

# Dev Setup
For development we reccomend creating a folder `PykaDex-Organisation` and then cloning each of the repos you plan to work on into into that directory. We reccomend this as alot of the repos will gathergenerated files from one another using relative file paths.

```bash
mkdir PykaDex-Organisation
cd PykaDex-Organisation
git clone git@github.com:PykaDex/PykaDex_Data.git
git clone git@github.com:PykaDex/PykaDex_Trainer.git
git clone git@github.com:PykaDex/PykaDex_WTP.git
```

## Some dev info
- Python3.6-3.7 using pytorch to train models
- streamlit to host api/web front
- c++ to develop dsi homebrew
- java/koitlin using android studio for android app
- kaggle images as base data set with some manual cleaning before augmentation

# progress
We currently have a good working foundation for the project, where we can train, test, manipulate the data. And have even successfully got web front end up (currently uses an untrained vg16 model, but can be tested online [here](https://share.streamlit.io/pykadex/pykadex_api/main) by simply uploading an image.
