# Setup CI/CD with Github Actions and Expo (eas)

WIP README

1. setup project with `expo`
1. add globally `expo-cli` and `eas-cli`
1. install `jest` with `expo install jest-expo jest`
1. add jest commands and config in `app.json`
1. configure eas by running `eas build:configure`
1. remove development client from `eas.json`, we're not using that
1. head to `expo.dev` and create an account along with a project
1. follow the steps to associate the project with the account
   1. change the slug in `app.json` to match the one given by `expo.dev`
   1. change the owner in `app.json` to match the one given by `expo.dev`
1. run `eas build` once in the terminal to connect to the `eas` service and manage the certificates needed for the build.
1. create GitHub repo and push the project to GitHub
1. Add the workflow
1. Configure the `EXPO_TOKEN` in Github Secrets
   1. Head to `expo.dev` **Account Settings > Access Token > Create**
   1. Copy & Paste the token on Github Secrets with the name `EXPO_TOKEN`
1. You should be good to go to build the project in CI
