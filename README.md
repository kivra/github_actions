# 🚀 Github Actions for Kivra's Frontend Projects

In this project we store our Github Actions that are shared between our different frontend applications.

## 🙋‍♂️ Frequently asked questions

### Q: How do I test my custom Github Action?

It's definitely possible to test the Github Action before merging into `main`.

1. Create your branch in the `github_actions` repository and push the code to Github.
2. In the project that you wish to use your action you can now point out the action with the SHA of the latest commit for your branch.

```yml
steps:
  - uses: kivra/github_actions/your-action@172239021f7ba04fe7327647b213799853a9eb89
```

_Note: Remember that if you do changes in your action, you'll need to update the SHA._
