# circleci
This project is part of an interview assignment for CircleCI. The document [workspacesvscaching.md](workspacesvscaching.md) covers the differences between Workspaces and Caching on CircleCI.

The section on [Caches, Workspaces, and Artifacts](https://circleci.com/docs/2.0/concepts/#caches-workspaces-and-artifacts) was used as a reference for this technical document.

## Building on CircleCI
The hidden `circleci` directory contains a [`config.yml`](https://github.com/annabaker/circleci/blob/main/.circleci/config.yml) file necessary for building on the 2.x CircleCI infrastructure. The sample configuration file uses the welcome [orb](https://circleci.com/docs/2.0/orb-intro/#quick-start), a Hello World configuration example.

To run, ensure your account is integrated with [Github](https://circleci.com/docs/2.0/gh-bb-integration/) and clone the `circleci` project.

Navigate to the Projects tab in the left-hand panel under your dashboard view. Select the **Set Up Project** button.

After selecting the Set Up Project button, you will be brought to the `config.yml` file mentioned previously. Select the **Use Existing Config** button and then select the **Start Building** button to build the project.
