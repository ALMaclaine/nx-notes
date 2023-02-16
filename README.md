# nx pitch notes

## What is nx
- enterprise monorepo orchestration tooling and SAAS
- created by ex-Google engineers (Angular Maintainer) based on Google's Bazel

## Problems to solve
- project tooling/dependency management
  - nx manages all main project tooling/configuration and dependencies
  - this frees developers from having to spend time researching the correct combination of dependencies that all work together
- task running
  - nx has built in task runner with advanced coordination abilities and caching
  - replaces ad hoc script running tooling with integrated task runners that understand the projects structure
- ability to break project apart into modularized packages that can be combined in arbitrary manners
  - nx helps generate and orchestrate modularized node packages
  - facilitates breaking app apart by feature, by page, by domain/subdomain
  - facilitates micro front ends
  - modularizing and recombining packages to form the application allows for adept architectural changes. (i.e. moving from react router to nextjs)
  - facilitates scoped development using storybook, features can be developed in isolation and then integrated into main app
- long build/test cycles
  - nx caches build results which can be shared amongst developers and ci/cd platforms
  - dependency graph analysis, test/build only what changed
  - incremental builds, build sub packages into final result, avoid re-building unchanged code
- understanding structure of large code base
  - by breaking project into many packages, we can trace the interconnections using dependency graph analysis
  - visualize code structure using graphs
  - facilitates operating on the affected path
- lack of resources to look to when problems occur with tooling
  - nrwl the creators of NX are also a consulting company, you can pay them to help with whatever problems you're facing 

## resources
- [nx techcrunch](https://techcrunch.com/2022/11/17/with-8-6m-in-seed-funding-nx-wants-to-take-monorepos-mainstream)
- [illustrated dte](https://nx.dev/more-concepts/illustrated-dte)
- [Micro Front Ends](https://techblog.geekyants.com/building-a-micro-frontend-using-react-and-angular)
- [Why Monorepos?](./why-monorepos.md)

## demos
- [large monorepo](https://github.com/vsavkin/large-monorepo)
- [dte](https://github.com/vsavkin/lerna-dte)

## DTE Image
![image](https://user-images.githubusercontent.com/16461670/219460948-da59f9f0-cdf9-480b-ab81-2580fdda9439.png)
