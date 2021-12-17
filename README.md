# gh-repos

- Create list of specific user's public repos as json and csv
  - `<user>..full.json`, `<user>.summarized.json`, `<user>.csv`
- Improved version of [eggplants/gh-matome](https://github.com/eggplants/gh-matome)

## Install

```bash
gh extension install eggplants/gh-repos
```

## Requirements

- [curl/curl](https://github.com/curl/curl)
- [stedolan/jq](https://github.com/stedolan/jq)

## Usage

```bash
gh repos <gh-username>
```

## Run Example

```shellsession
$ gh repos eggplants
created: 'eggplants.full.json', 'eggplants.summarized.json', 'eggplants.csv'
$ head eggplants.full.json; echo ...
[
  {
    "id": 394622349,
    "node_id": "MDEwOlJlcG9zaXRvcnkzOTQ2MjIzNDk=",
    "name": "-scenario",
    "full_name": "eggplants/-scenario",
    "private": false,
    "owner": {
      "login": "eggplants",
      "id": 42153744,
...
$ head eggplants.csv; echo ...
"index","name","description","lang","fork","archived","star","created","updated"
"0","f_down","futaba channel thread downloader via tsumanne","Ruby","false","true","1","2018-12-15T20:01:05Z","2020-12-17T18:13:34Z"
"1","18_prog2","my answers in the class of ""Computer Programming Lab Ⅱ.""","Ruby","false","true","0","2019-01-19T07:24:36Z","2020-01-11T07:35:49Z"
"2","markdowns","This stores my useless markdown files...","HTML","false","false","0","2019-01-24T14:53:55Z","2020-01-26T00:55:09Z"
"3","eng_vocab","https://eggplants.github.io/eng_vocab/","HTML","false","true","0","2019-01-29T15:42:11Z","2020-03-29T20:25:18Z"
"4","weblio_scrape","fetch the data from ""https://ejje.weblio.jp/"" & scrape it","Ruby","false","false","0","2019-01-31T20:52:22Z","2019-09-14T13:34:14Z"
"5","twitter_app","おもちゃ","Python","false","false","1","2019-05-19T21:32:11Z","2020-05-18T23:47:26Z"
"6","opac","Exercises for ""Knowledge and Information Practice"": Building OPAC","CSS","false","true","0","2019-06-23T13:40:18Z","2021-09-06T11:35:27Z"
"7","meyasu",,"PHP","false","true","0","2019-07-11T06:33:33Z","2020-04-26T13:55:10Z"
"8","gpa",,"Shell","false","false","0","2019-07-23T10:35:40Z","2019-12-10T18:17:54Z"
...
```

## License

MIT
