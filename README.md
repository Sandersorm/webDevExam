# WAD 2020 Resit Exam: Project B

## Project setup
```
npm install
```

### Run your tests
```
npm run test
```
# Setup

You will need to [import](https://docs.github.com/en/free-pro-team@latest/github/importing-your-projects-to-github/importing-a-repository-with-github-importer) 
this repository to you GitHub account, to do that please follow these steps:
* Go to Github [import page](https://github.com/new/import)
  * **Note**: you have to be logged in to your GitHub account
* In the first field `"Your old repository’s clone URL"` enter URL of this repository `https://github.com/tsotnekekelia/wad20-exam3-b`
* In  the next field give it a name
* Make it **Private**
* And begin to import, it should take few seconds
* Add me as a collaborator to your new repository, [click here](https://docs.github.com/en/free-pro-team@latest/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository)
 to learn how
  * My `email` and `username` on github is: `cotne.kekelia@yahoo.com` and `tsotnekekelia`
  
# Tasks
  
Modify [Bets.spec.js](tests/unit/Bets.spec.js) 
to test the functionality of [Bets.vue](src/components/Bets.vue) component.
 
**Note:** you need to create and pass some test data to this component in the test file.

1. Test that as many bets are displayed as items in the array that are passed to `Bets` component; One bet is encapsulated in a `tr` with class `.bet` _**[9 points]**_
2. Test that `.win` and `.lose` classes are properly attached to the bet with the appropriate `result` _**[9 points]**_
3. Test that final total is correctly calculated (sum of winnings  - sum of amounts of lost bets) _**[7 points]**_
  
