# AesopDocs
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FAesopDocs%2Faesopdocs-action.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FAesopDocs%2Faesopdocs-action?ref=badge_shield)

AesopDocs is a GitHub action used to automatically generate documentation for your repo. 

If you add it as part of your GitHub Actions workflows, upon activating the trigger mechanism
that you specify, it will go over your repository, generate UML and class diagrams, generate 
high-level documentation and create a PR for it. 

Additional configuration options allow you to select whether you'd like it to also produce docstring
for any modified or newly introduced methods and/or classes.

### Set-up instructions
As a bear minimum you need to provide a valid GITHUB_ACCESS_TOKEN for AesopDocs to be able to interact
with your repo. 

Here are the required permissions:
### TODO
- specify minimal set of permission required on access token
- Required input and output arguments
- Optional input and output arguments
- Environment variables the action uses

Here's a simple example of how you can use this as part of an existing GitHub Actions workflow:
```bash
steps:
  - name: Generate docs
    uses: actions/aesopdocs-action@v1
    with: 
      branch: 'main'
      github_access_token: ${{ secrets.ACCESS_TOKEN }}
```

Here's another example with illustrating the use of the additional options you can use to configure it
```bash
TODO add example here
```

## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FAesopDocs%2Faesopdocs-action.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FAesopDocs%2Faesopdocs-action?ref=badge_large)