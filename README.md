# MEOM data catalog

This repo contains the sources for the [MEOM data catalog](https://meom-group.github.io/meom-data-catalog)

All the extractions informations are gathered in one yaml file : _data/extractions.yml
If you want to add a new one just copy paste the structure of another dataset, the mandatory informations are :

  - name
  - configuration
  - simulation
  - region
  - variable
  - period
  - frequency

All the other are optionnal

If the dataset you are adding is about a new [configuration, simulation, region, variable and/or platform (you can check if this is the case by looking at the [comprehensive list](https://meom-group.github.io/meom-data-catalog/), you will need to add an extra category by duplicating an existing one in two place :
  - in content/category, you duplicate an existing markdown file
  - in _includes, you duplicate an existing list_extract_xxxx.html corresponding to the same category

The structure is inspired by [this template](https://github.com/learn-static/lesson-template)
