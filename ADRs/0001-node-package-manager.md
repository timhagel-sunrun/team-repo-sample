# 0001 Node package manager 

## Status

Approved / Declined

## Context

We want to decide whether or not to use npm or yarn for managing packages in a node project. Traditionally the team has used Yarn because it provided many benefits that npm did not have. We want to reevaluate that decision now that npm has gotten more 

## Decision

We decided to switch over to npm because it has all of the features we want and is a more directly supported default option. This benefit outweighs the disadvantage of the slower install time.

## Options

### Use NPM

Use npm directly for installing and managing packages.

- Good
  - Industry standard default option.
  - Comes with node installation.
- Bad
  - Installs synchronously (slower)
  - Existing customer repositories are using yarn. So we would either have to migrate them or live with the inconsistency until we can do so.

### Use Yarn

We can continue using yarn

- Good
  - Most popular alternative to npm
  - Installs packages asynchronously (fast)
- Bad
  - Yarn has to be installed separately from node
  - 

## Additional Resources

Add links for additional information