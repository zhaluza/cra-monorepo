# CRA-Monorepo

### Summary

An example of a simple frontend monorepo containing a React app and a folder of shared components.
This pattern can be used to create a component library used by other apps or microfrontends
contained in the same repo.

### Tech

- Both packages were bootstrapped with [Create React App](https://create-react-app.dev/) using the
  [TypeScript template](https://create-react-app.dev/docs/adding-typescript/).
- Linked with [Yarn workspaces](https://classic.yarnpkg.com/en/docs/workspaces/).
- To access files outside its own `src` directory, the React app (`app-1`) uses
  [react-app-rewired](https://www.npmjs.com/package/react-app-rewired) and
  [customize-cra](https://www.npmjs.com/package/customize-cra) to bypass CRA's restrictions against
  importing external files.
