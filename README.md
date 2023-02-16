# nx pitch notes

## Index
[Why Monorepos?](./why-monorepos.md)

## problems to solve
- project tooling/dependency management
  - nx manages all main project tooling/configuration and dependencies
- task running
  - nx has built in task runner with advanced coordination abilities and caching
- ability to break project apart into modularized packages that can be combined in arbitrary manners
  - nx helps generate and orchestrate modularized node packages
  - facilitates breaking app apart by feature, by page, by domain/subdomain
  - facilitates micro front ends
- long build/test cycles
  - nx caches build results which can be shared amongst developers and ci/cd platforms
  - dependency graph analysis, test/build only what changed
  - incremental builds, build sub packages into final result, avoid re-building unchanged code 

## resources
- [nx techcrunch](https://techcrunch.com/2022/11/17/with-8-6m-in-seed-funding-nx-wants-to-take-monorepos-mainstream)
- [illustrated dte](https://nx.dev/more-concepts/illustrated-dte)
- [Why monorepo](https://nx.dev/more-concepts/why-monorepos)
- [Micro Front Ends](https://techblog.geekyants.com/building-a-micro-frontend-using-react-and-angular)

## demos
- [large monorepo](https://github.com/vsavkin/large-monorepo)
- [dte](https://github.com/vsavkin/lerna-dte)

## DTE Image
![image](https://user-images.githubusercontent.com/16461670/219460948-da59f9f0-cdf9-480b-ab81-2580fdda9439.png)
