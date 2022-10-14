# GitHub Action for Joxi

> Learn more about [joxi](https://github.com/onmax/joxi)

## Set up

1. [Fork](https://github.com/onmax/joxi-github-action/fork) this repository.
2. Create all the enviromental variables explained in the [Setup instructions](https://github.com/onmax/joxi#setup).
3. Give access to GitHub actions to access those variables in the `Actions secrets` panels inside `Settings`.
	- Specifically, inside `Settings` > `Secrets` > `Actions secrets` you should have the enviromental variables.
3. Update the GitHub Actions configuration. Make sure to select a trigger for the GitHub Action that is commented. For that, read the instructions in line 5. As an example, if I want to have both triggers, I would have something like (removed comments for simplicity):

```yml
on:
  schedule:
    - cron: "07 */24 * * *"
  workflow_dispatch:
```

> It is recommendable that you change the visibility of your fork to `hidden`, but this comes with some drawbacks.

## How to update

You can always comeback to [this repo](https://github.com/onmax/joxi-github-action) and manually copy and paste the GitHub Action.

